---
title: Настройка уведомлений об изменениях, включающих данные ресурсов
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления об изменениях могут включать свойства ресурсов.
author: Jumaodhiss
ms.prod: non-product-specific
ms.localizationpriority: high
ms.openlocfilehash: 9bbd29d374160fdd8c86b6bd34293ce7fe241e17
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898828"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a>Настройка уведомлений об изменениях, включающих данные ресурсов

Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md). Вы можете настроить подписки таким образом, чтобы в уведомления об изменениях включались данные измененных ресурсов (например, содержимое сообщения чата из Microsoft Teams или сведения о присутствии из Microsoft Teams). Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса. В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.

Добавление данных ресурса в уведомления об изменениях требует реализации следующей дополнительной логики, чтобы выполнить требования по доступу к данным и их безопасности. 

- [Применяйте](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications) специальные уведомления жизненного цикла подписки, чтобы обеспечить непрерывный поток данных. Microsoft Graph периодически отправляет уведомления жизненного цикла, требуя от приложения повторной авторизации, чтобы обеспечить отсутствие неожиданных проблем с доступом при включении данных ресурсов в уведомления об изменениях.
- [Проверяйте](#validating-the-authenticity-of-notifications) подлинность уведомлений об изменениях, подтверждая что их источником является Microsoft Graph.
- [Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных в уведомлениях об изменениях.

## <a name="resource-data-in-notification-payload"></a>Сведения ресурсов в полезных данных уведомлений

Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.

- Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.
- Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.
- Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**. Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.  


## <a name="supported-resources"></a>Поддерживаемые ресурсы

Ресурсы Microsoft Teams [chatMessage](/graph/api/resources/chatmessage), [onlineMeetings](/graph/api/resources/onlinemeeting) и [presence](/graph/api/resources/presence) поддерживают уведомления об изменениях данных ресурсов. Ресурсы Outlook [contact](/graph/api/resources/contact.md), [event](/graph/api/resources/event.md) и [message](/graph/api/resources/message.md) имеют аналогичную поддержку _в предварительной версии_. В частности, вы можете настроить подписку для вариантов использования, перечисленных ниже.

Доступно в конечных точках v1.0 и бета-версии:
- Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`
- Новые или измененные сообщения во всех каналах Teams всей организации (клиент): `/teams/getAllMessages`
- Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`
- Новые или измененные сообщения во всех чатах Teams: `/chats/getAllMessages`
- Новые или измененные участники во всех чатах Teams: `/chats/getAllMembers`
- Новые или измененные участники в определенном чате Teams: `/chats/{id}/members`
- Новый или измененный чат во всем клиенте: `/chats`
- Изменения свойств в определенном чате: `/chats/{id}`
- Новые или измененные участники во всех каналах в определенной команде: `/teams/{id}/channels/getAllMembers`
- Новые или измененные участники в определенной команде: `/teams/{id}/members`
- Новая или измененная команда во всем клиенте: `/teams`
- Изменения свойств в определенной команде: `/teams/{id}`
- Новые или измененные каналы во всех командах Teams: `/teams/getAllChannels`
- Новый или измененный канал в определенной команде: `/teams/{id}/channels`
- Обновление сведений о присутствии пользователя: `/communications/presences/{id}`

Доступно только в конечной точке бета-версии:
- Новые или измененные личные контакты в почтовом ящике пользователя: `/users/{id}/contacts`
- Новые или измененные личные контакты в contactFolder пользователя: `/users/{id}/contactFolders/{id}/contacts`
- Новые или измененные события в почтовом ящике пользователя: `/users/{id}/events`
- Новые или измененные сообщения в почтовом ящике пользователя: `/users/{id}/messages`
- Новые или измененные сообщения в mailFolder пользователя: `/users/{id}/mailFolders/{id}/messages`
- Обновления сведений о состоянии собрания Teams:`/communications/onlineMeetings/{meeting-id}`

Уведомления об изменениях, которые включают данные ресурса **chatMessage**, **onlineMeeting** или **presence**, содержат все свойства измененного экземпляра. Они не поддерживают возвращение только выбранных свойств экземпляра. 

Уведомления об изменениях для ресурсов **contact**, **event** или **message** включают только подмножество свойств ресурса, которые должны быть указаны в соответствующем запросе на подписку с помощью параметра запроса `$select`. Дополнительные сведения и пример подписки на уведомления об изменениях с данными ресурса для ресурса **message** см. в статье [Изменение уведомлений для ресурсов Outlook в Microsoft Graph](outlook-change-notifications-overview.md). 

В оставшейся части этой статьи рассматривается пример подписки на уведомления об изменениях для ресурсов **chatMessage** в канале Teams, при этом каждое уведомление об изменении включает полные данные ресурса измененного экземпляра **chatMessage**. Дополнительные сведения о подписках на основе объекта **chatMessage** см. в статье [Получение уведомлений об изменениях сообщений чатов и каналов](teams-changenotifications-chatmessage.md).

## <a name="creating-a-subscription"></a>Создание подписки

Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):

- **includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.
- **encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса. Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата. Используйте этот идентификатор для определения в каждом уведомлении об изменениях сертификата, используемого для расшифровки.

Учитывайте следующее:

- Проверьте обе конечные точки, как описано в ст. [Проверка конечной точки уведомлений](webhooks.md#notification-endpoint-validation). Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.

### <a name="subscription-request-example"></a>Пример запроса на подписку

В приведенном ниже примере показано, как подписаться на сообщения канала, созданные или обновляемые в Microsoft Teams.

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a>Отклик подписки
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a>Уведомления жизненного цикла подписки

Некоторые события могут воздействовать на поток уведомлений об изменениях в существующей подписке. Уведомления жизненного цикла подписки указывают необходимые действия для обеспечения непрерывного потока. В отличие от уведомления об изменении ресурса, информирующем об изменении экземпляра ресурса, уведомление жизненного цикла относится к самой подписке и ее текущему состоянию в жизненном цикле. 

Дополнительные сведения о том, как получать уведомления в жизненном цикле, а также отвечать на них, см. в статье [Уменьшение количества пропущенных уведомлений о подписках и изменениях](webhooks-lifecycle.md)

## <a name="validating-the-authenticity-of-notifications"></a>Проверка подлинности уведомлений

Приложения часто запускают бизнес-логику на основе данных ресурсов, включенных в уведомления об изменениях. Важно сначала проверить подлинность каждого уведомления об изменениях. В противном случае посторонние смогут обмануть ваше приложение с помощью ложных уведомлений об изменениях, заставить его неправильно выполнять бизнес-логику, что приведет к нарушению безопасности.

Для основных уведомлений об изменениях, не содержащих данные ресурсов, просто проверьте их на основе значения **clientState**, как описано здесь [Обработка уведомлений об изменениях](webhooks.md#processing-the-change-notification). Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено. 

Для уведомлений об изменениях, доставляющих данные ресурсов, проведите более тщательную проверку перед обработкой данных.

Содержание:

- [Маркеры проверки в уведомлении об изменениях](#validation-tokens-in-the-change-notification)
- [Способ проверки](#how-to-validate)
- [Пример маркера JWT](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a>Маркеры проверки в уведомлении об изменениях

Уведомление об изменениях с данными ресурсов содержит дополнительное свойство **validationTokens**, содержащее массив маркеров JWT, созданных Microsoft Graph. Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**. Учитывайте, что уведомления об изменениях могут содержать разные элементы для различных приложений и клиентов, подписанных с помощью одинакового значения **notificationUrl**.

> **Примечание.** Если вы настраиваете [доставку уведомлений об изменениях через Центры событий Azure](change-notifications-delivery.md), Microsoft Graph не будет отправлять маркеры проверки. Microsoft Graph не требуется проверять **notificationUrl**.


В следующем примере уведомление об изменении содержит два элемента для одного приложения и двух разных клиентов, поэтому массив **validationTokens** содержит два маркера, требующих проверки.

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```

> **Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="how-to-validate"></a>Способ проверки

Если вы незнакомы с проверкой маркеров, см. обзор в статье [Принципы проверки маркера](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/). Используйте пакет SDK, например библиотеку [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) для .NET или стороннюю библиотеку для другой платформы.

Следует учитывать следующее: 

- Всегда отправляйте код состояния `HTTP 202 Accepted` в ответе на уведомление об изменении. 
- Дайте ответ перед проверкой уведомления об изменении (например, если вы храните уведомления об изменениях в очередях для последующей обработки) или после нее (если они обрабатываются на ходу), даже если проверка завершилась сбоем.
- Принятие уведомления об изменении позволяет избежать ненужных повторений доставки, а также мешает любым возможным злоумышленникам выяснить, прошли ли они проверку. Вы всегда можете игнорировать неверное уведомление об изменении после его принятия.

В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**. Если любой из маркеров не прошел проверку, считайте уведомление об изменении подозрительным и выполните дальнейшее исследование. 

Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.

1. Убедитесь, что срок действия маркера не истек.

2. Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (платформой удостоверений Майкрософт для разработчиков):

    - Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`. Эта конфигурация кэшируется приложением на определенный период времени. Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.
    - Проверьте подпись маркера JWT, использующего эти ключи.

    Не принимайте маркеры, выпущенные любыми другими центрами.

3. Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.

    Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции. 
    - Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.
    - Если уведомления об изменениях получают несколько приложений, выполните проверку по нескольким идентификаторам.


4. **Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph. 

    - Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.
    - Это гарантирует, что уведомления об изменениях не отправляются другим приложением, отличным от Microsoft Graph.


### <a name="example-jwt-token"></a>Пример маркера JWT

Ниже приведен пример свойств, входящих в маркер JWT, которые требуется проверить.

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a>Пример: подтверждение маркеров проверки

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
Чтобы пример Java работал, вам также необходимо реализовать `JwkKeyResolver`.  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a>Расшифровка данных ресурсов из уведомлений об изменениях

Свойство **resourceData** уведомления об изменении содержит только основной идентификатор и сведения о типе экземпляра ресурса. Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке. Это свойство также содержит значения, необходимые для проверки и расшифровки. Это выполняется для повышения безопасности пользовательских данных, к которым получен доступ с помощью уведомлений об изменениях. Вы отвечаете за защиту закрытого ключа, чтобы гарантировать невозможность расшифровки пользовательских данных посторонними, даже если они смогли перехватить исходные уведомления об изменениях.

Содержание:

- [Управление ключами шифрования](#managing-encryption-keys)
- [Расшифровка данных ресурсов](#decrypting-resource-data)
- [Пример: расшифровка уведомления с зашифрованными данными ресурсов](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>Управление ключами шифрования

1. Получите сертификат с парой асимметричных ключей.

    - Вы можете самостоятельно подписать сертификат, так как Microsoft Graph не проверяет поставщика сертификата и использует открытый ключ только для шифрования. 
    - В качестве решения для создания и ротации сертификатов, а также безопасного управления ими используйте [Azure Key Vault](/azure/key-vault/key-vault-whatis). Убедитесь, что ключи удовлетворяют следующим условиям:

        - Ключ должен быть типа `RSA`
        - Размер ключа должен находиться в диапазоне от 2048 до 4096 бит

2. Экспортируйте сертификат в формате X.509 с кодировкой base64 и **добавьте только открытый ключ**. 

3. При создании подписки:

    - Укажите сертификат в свойстве **encryptionCertificate**, используя контент в кодировке base64, в которой сертификат был экспортирован.
    - Укажите ваш собственный идентификатор в свойстве **encryptionCertificateId**. 
  
        Этот идентификатор позволяет сопоставлять сертификаты с получаемыми уведомлениями об изменениях, а также получать сертификаты из хранилища сертификатов. Длина идентификатора не должна превышать 128 символов.

4. Обеспечьте защиту закрытого ключа, чтобы ваш код обработки уведомлений об изменениях мог обращаться к закрытому ключу для расшифровки данных ресурсов.

#### <a name="rotating-keys"></a>Ротация ключей

Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи. Чтобы добавить новую пару ключей, выполните следующие действия:

1. Получите новый сертификат с новой парой асимметричных ключей. Используйте его для всех создаваемых подписок.

2. Обновите существующие подписки с использованием нового ключа сертификата.

    - Выполняйте это в рамках регулярного возобновления подписки. 
    - Или перечислите все подписки и укажите ключ. Используйте [операцию PATCH для подписки](/graph/api/subscription-update) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.

3. Учитывайте следующее:
    - В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования. Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.
    - Используйте свойство **encryptionCertificateId** в каждом уведомлении об изменении, чтобы определить правильный ключ для использования.
    - Удалите старый сертификат, только когда он перестает указываться в последних уведомлениях об изменениях.

### <a name="decrypting-resource-data"></a>Расшифровка данных ресурсов

Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:
  - Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.
  - Используется открытый асимметричный ключ (указанный при подписке), чтобы зашифровать симметричный ключ и добавить его в каждое уведомление об изменении этой подписки.

Всегда предполагайте, что для каждого элемента в уведомлении об изменении используется разный симметричный ключ.

Чтобы расшифровать данные ресурсов, приложение должно выполнить обратные действия, используя свойства в разделе **encryptedContent** в каждом уведомлении об изменении:

1. Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.

2. Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8&preserve-view=true)) с помощью закрытого ключа.

3. Расшифруйте симметричный ключ, указанный в свойстве **dataKey** каждого элемента в уведомлении об изменении.

    Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.

4. Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.
  
    Сравните его со значением в объекте **dataSignature**. Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.

5. Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8&preserve-view=true)) для расшифровки содержимого в объекте **data**.

    - Используйте следующие параметры расшифровки для алгоритма AES:

        - Дополнение: PKCS7
        - Режим шифрования: CBC
    - Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.

6. Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении об изменении.


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>Пример: расшифровка уведомления с зашифрованными данными ресурсов

Ниже приведен пример уведомления об изменении, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала. Экземпляр определяется значением `@odata.id`.

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

> **Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).


В этом разделе содержатся некоторые полезные фрагменты кода, использующие C# и .NET для каждого этапа расшифровки.

#### <a name="decrypt-the-symmetric-key"></a>Расшифровка симметричного ключа

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a>Сравнение подписи данных с помощью HMAC-SHA256

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a>Расшифровка содержимого данных ресурсов

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a>См. также

- [Настройка уведомлений об изменениях в пользовательских данных](webhooks.md)
- [Тип ресурса subscription](/graph/api/resources/subscription)
- [Получение подписки](/graph/api/subscription-get)
- [Создание подписки](/graph/api/subscription-post-subscriptions)
- [Обновление подписки](/graph/api/subscription-update)
- [Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph](outlook-change-notifications-overview.md)
