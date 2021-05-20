---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: resourcePageType
ms.openlocfilehash: 4ceb5a98fd330efa3b5e9b8b62d32598b5972984
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547585"
---
# <a name="subscription-resource-type"></a>Тип ресурса subscription

Пространство имен: microsoft.graph

Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.

- [Оповещение][] Microsoft Graph Security API.
- Объект [callRecord][], создаваемый после звонка или собрания в Microsoft Teams.
- Объект [chatMessage][], отправленный в командах или каналах в Microsoft Teams.
- [Беседа][] в группе Microsoft 365.
- Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папки [driveItem][] в личном хранилище OneDrive пользователя.
- [Список][] на [сайте][] SharePoint.
- [Сообщение][], [событие][] или [контакт][] в Outlook.
- Объект [printer][] (когда задание печати для принтера переходит в состояние JobFetchable — готово к извлечению для печати) и [printTaskDefinition][] универсальной печати. Дополнительные сведения см. в статье [Подписка на уведомления об изменениях из API облачной печати](/graph/universal-print-webhook-notifications).
- [Пользователь][] или [группа][] в Azure Active Directory.

Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Обновление подписки путем изменения ее срока действия. |
| [Перечисление подписок](../api/subscription-list.md) | [subscription](subscription.md) | Перечисление активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойств и связей объекта subscription. |
| [Удаление подписки](../api/subscription-delete.md) | Нет | Удаление объекта subscription. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание | Поддерживаемые ресурсы |
|:---------|:-----|:------------|:--------------|
| changeType | string | Обязательный. Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.<br><br>Примечание. Уведомления об изменении корневых элементов диска и списков поддерживают только changeType `updated`. Уведомления об изменении пользователей и групп поддерживают changeType `updated` и `deleted`. | Все |
| notificationUrl | string | Обязательный. URL-адрес конечной точки, которая будет получать уведомления об изменениях. Этот URL-адрес должен использовать протокол HTTPS. | Все |
| lifecycleNotificationUrl | string | URL-адрес конечной точки, принимающей уведомления жизненного цикла, в том числе уведомления `subscriptionRemoved` и `missed`. Этот URL-адрес должен использовать протокол HTTPS. Необязательно. <br><br>[Дополнительные сведения](/graph/webhooks-lifecycle) об использовании уведомлений жизненного цикла ресурсами Outlook. | Все |
| resource | string | Обязательное. Указывает ресурс, для которого будут отслеживаться изменения. Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`). См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.| Все |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Обязательное. Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.  В приведенной ниже таблице указан максимально допустимый период подписки. | Все |
| clientState | string | Необязательно. Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении об изменении. Максимальная длина — 128 символов. Клиент может проверить, пришло ли уведомление об изменении от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением об изменении. | Все |
| id | string | Уникальный идентификатор для подписки. Только для чтения. | Все |
| applicationId | string | Идентификатор приложения, использованного для создания подписки. Только для чтения. | Все |
| creatorId | string | Идентификатор пользователя или субъекта-службы, которые создали подписку. Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение. Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению. Только для чтения. | Все |
| includeResourceData | Boolean | Если присвоено значение `true`, уведомления об изменениях [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата). Необязательно. | Все |
| encryptionCertificate | string | Представление в кодировке Base64 сертификата с открытым ключом, используемое для шифрования данных ресурса в уведомлениях об изменениях. Необязательно. Обязательно, если **includeResourceData** имеет значение true. | Все |
| encryptionCertificateId | string | Предоставляемый приложением настраиваемый идентификатор, помогающий определить сертификат, необходимый для расшифровки данных ресурса. Необязательный.| Все |
| latestSupportedTlsVersion | Строка | Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**. Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2. Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем. </br></br>Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна. В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`. | Все |
| notificationContentType | строка | Нужный тип контента для уведомлений об изменениях MS Graph для поддерживаемых типов ресурсов. Тип контента по умолчанию — "application/json". | Все |
| notificationQueryOptions | строка | Параметры запросов OData для указания значения целевого ресурса. Клиенты получают уведомления, когда ресурс переходит в состояние, соответствующее указанным здесь параметрам запроса. Благодаря этому новому свойству в полезных данных создания подписки, а также существующим свойствам, веб-перехватчики будут предоставлять уведомления, когда ресурс достигает нужного состояния, указанного в свойстве notificationQueryOptions, например когда завершается задание печати, когда значение свойства `isFetchable` ресурса задания печати принимает значение true и т. д. | [Служба универсальной печати](/graph/universal-print-webhook-notifications) |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Максимальный период подписки для каждого из типов ресурсов

| Ресурс            | Максимальный срок действия  |
|:--------------------|:-------------------------|
| **Оповещение** безопасности     | 43200 минут (до 30 дней)  |
| **callRecord** в Teams    | 4230 минут (до 3 дней)  |
| **chatMessage** в Teams    | 60 минут (1 час)  |
| Групповая **беседа** | 4230 минут (до 3 дней)    |
| **driveItem** OneDrive    | 4230 минут (до 3 дней)    |
| **Список** SharePoint    | 4230 минут (до 3 дней)    |
| **Сообщение**, **событие**, **контакт** Outlook              | 4230 минут (до 3 дней)    |
| **Пользователь**, **группа**, другие ресурсы каталога   | 4230 минут (до 3 дней)    |
| **printer** печати | 4230 минут (до 3 дней)    |
| **printTaskDefinition** печати | 4230 минут (до 3 дней)    |


> **Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение. В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

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

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string",
  "notificationContentType": "string",
  "notificationQueryOptions": "string"
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
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;"
}-->

