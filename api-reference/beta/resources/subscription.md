---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 70bc8842ed3ccda835e836c5e4c9337668e54ec8
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368107"
---
# <a name="subscription-resource-type"></a>Тип ресурса subscription

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. В настоящее время подписки включены для следующих ресурсов.

> **Примечание** Подписки, отмеченные звездочкой (*), поддерживаются только в конечной `/beta` точке.

- [Оповещение][] Microsoft Graph Security API.
- Объект [callRecord][], создаваемый после звонка или собрания в Microsoft Teams.
- Канал [в](./channel.md) Microsoft Teams.*
- Чат [в](./chat.md) Microsoft Teams.*
- Объект [chatMessage][], отправленный в командах или каналах в Microsoft Teams.
- [Беседа][] в группе Microsoft 365.
- [ConversationMember в](./conversationmember.md) команде, канале или чате в Microsoft Teams.*
- Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папки [driveItem][] в личном хранилище OneDrive пользователя.
- [Группа][] в Azure Active Directory.
- [Список][] на [сайте][] SharePoint.
- [Сообщение][], [событие][] или [контакт][] в Outlook.
- [Онлайн-собрание][] в Microsoft Teams.*
- Присутствие [пользователя][] в Microsoft Teams.*
- Команда [в](./team.md) Microsoft Teams.*
- Объект [printer][] (когда задание печати для принтера переходит в состояние JobFetchable — готово к извлечению для печати) и [printTaskDefinition][] универсальной печати. Дополнительные сведения см. в статье [Подписка на уведомления об изменениях из API облачной печати](/graph/universal-print-webhook-notifications).
- [BaseTask][] пользователя в Microsoft To Do.*
- [Пользователь][] в Azure Active Directory.

О возможных значениях пути ресурсов для каждого поддерживаемого ресурса и о том, как ресурсы используют уведомления жизненного цикла, см. раздел [ Использовать Microsoft Graph API для получения уведомлений об изменениях](webhooks.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Обновив подписку, обновив срок ее действия. |
| [Перечисление подписок](../api/subscription-list.md) | [subscription](subscription.md) | Перечисление активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойств и связей объекта подписки. |
| [Удаление подписки](../api/subscription-delete.md) | Нет | Удаление объекта подписки. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание | Поддерживаемые ресурсы |
|:---------|:-----|:------------|:--------------|
| applicationId | String | Необязательный параметр. Идентификатор приложения, использованного для создания подписки. Только для чтения.  | Все |
| changeType | Строка | Обязательный. Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми. <br><br>**Примечание.** <li> Уведомления об изменении корневого элемента диска и списка поддерживают только changeType `updated`. <li>Уведомления об изменении [пользователей](../resources/user.md) и [групп](../resources/user.md) поддерживают changeType `updated` и `deleted`. | Все |
| clientState | String | Необязательный параметр. Указывает значение свойства **clientState** , отправленного службой в каждом уведомлении об изменении. Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного с каждым уведомлением об изменении. | Все |
| creatorId | String | Необязательный параметр. Идентификатор пользователя или субъекта-службы, которые создали подписку. Если приложение использовало делегирование разрешений для создания подписки, это поле содержит ID подписанного пользователя, созвали его от имени. Если приложение использовало разрешения приложения, это поле содержит ID основного владельца службы, соответствующего приложению. Только для чтения. | Все |
| encryptionCertificate | String | Необязательный параметр. Представление в кодировке Base64 сертификата с открытым ключом, используемое для шифрования данных ресурса в уведомлениях об изменениях. Необязательный, но необходимый при **includeResourceData** равном `true`. | Все |
| encryptionCertificateId | String | Необязательный параметр. Предоставляемый приложением настраиваемый идентификатор, помогающий определить сертификат, необходимый для расшифровки данных ресурса. Обязательно, **если включитьResourceData** является `true`. | Все |
| expirationDateTime | DateTimeOffset | Обязательное. Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка. Максимальное поддерживаемое время подписки см. [в таблице ниже](#maximum-length-of-subscription-per-resource-type).  | Все |
| id | String | Необязательный параметр. Уникальный идентификатор для подписки. Только для чтения. | Все |
| includeResourceData | Boolean | Необязательное свойство. Если присвоено значение `true`, уведомления об изменениях [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата). | Все |
| latestSupportedTlsVersion | String | Необязательный параметр. Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**. Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2. Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем. </br></br>Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна. В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`. | Все |
| lifecycleNotificationUrl | String | Необязательный параметр. URL-адрес конечной точки, принимающей уведомления жизненного цикла, в том числе уведомления `subscriptionRemoved` и `missed`. Этот URL-адрес должен использовать протокол HTTPS. | Все |
| notificationContentType | String | Необязательный параметр. Желаемый **тип контента** для уведомлений об изменении Microsoft Graph для поддерживаемых типов ресурсов. Тип контента по умолчанию – `application/json`. | Все |
| notificationQueryOptions | String |Необязательный параметр.  Параметры запроса OData для указания значения для целевого ресурса. Клиенты получают уведомления, когда ресурс достигает состояния, соответствующего предоставляемым здесь вариантам запроса. С помощью этого нового свойства в полезной нагрузке создания подписки наряду со всеми существующими свойствами веб-пользователи будут предоставлять уведомления всякий раз, когда ресурс достигнет нужного состояния, упомянутого в свойстве **notificationQueryOptions** . Например, по окончании печати или когда свойство ресурса печати `isFetchable` приобретает значение `true` и т.п. | [Служба универсальной печати](/graph/universal-print-webhook-notifications) |
| notificationUrl | Строка | Обязательный. URL-адрес конечной точки, которая получает уведомления об изменении. Этот URL-адрес должен использовать протокол HTTPS.  | Все |
| notificationUrlAppId| String | Необязательный параметр. ID приложения, который служба подписки может использовать для создания маркера проверки. Это позволяет клиенту проверить подлинность полученного уведомления.  | Все |
| resource | Строка | Обязательный. Указывает ресурс, для которого будут отслеживаться изменения. Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`). См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.  | Все |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Максимальный период подписки для каждого из типов ресурсов

| Ресурс            | Максимальный срок действия  |
|:--------------------|:-------------------------|
| **Оповещение** безопасности     | 43200 минут (до 30 дней)  |
| **callRecord** в Teams    | 4230 минут (до 3 дней)  |
| **Канал** Teams     | 60 минут (1 час)  |
| **Чат** Teams | 60 минут (1 час) |
| **chatMessage** в Teams    | 60 минут (1 час)  |
| **conversationMember** в Teams    | 60 минут (1 час)  |
| Teams **onlineMeeting** | 4320 минут (3 дня) |
| **Команда** Teams    | 60 минут (1 час)  |
| Групповая **беседа** | 4230 минут (до 3 дней)    |
| **driveItem** OneDrive    | 43200 минут (до 30 дней)    |
| **Список** SharePoint    | 43200 минут (до 30 дней)    |
| **Сообщение**, **событие**, **контакт** Outlook              | 4230 минут (до 3 дней)    |
| **Пользователь**, **группа**, другие ресурсы каталога   | 41 760 минут (до 29 дней)    |
| **presence**        | 60 минут (1 час) |
| **printer** печати | 4230 минут (до 3 дней)    |
| **printTaskDefinition** печати | 4230 минут (до 3 дней)    |
| **baseTask**              | 4230 минут (до 3 дней)    |


> **Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение. В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

``` json
{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "String (identifier)",
  "resource": "String",
  "changeType": "String",
  "clientState": "String",
  "notificationUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "applicationId": "String",
  "creatorId": "String",
  "includeResourceData": "Boolean",
  "lifecycleNotificationUrl": "String",
  "encryptionCertificate": "String",
  "encryptionCertificateId": "String",
  "latestSupportedTlsVersion": "String",
  "notificationQueryOptions": "String",
  "notificationContentType": "String",
  "notificationUrlAppId": "String"
}
```

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md
[callRecord]: ./callrecords-callrecord.md
[presence]: ./presence.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[baseTask]: ./basetask.md
[онлайн-собрание]: ./onlinemeeting.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


