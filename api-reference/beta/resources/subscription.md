---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: e34f6f04545c9f878e5429e54923ef223a883547
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934815"
---
# <a name="subscription-resource-type"></a>Тип ресурса subscription

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.

- [Оповещение][] Microsoft Graph Security API
- [callRecord][], создаваемый после звонка или собрания в Microsoft Teams
- Объект [chatMessage][], отправленный в командах или каналах в Microsoft Teams
- [Беседа][] в группе Microsoft 365 
- Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.
- [Список][] на [сайте][] SharePoint
- [Сообщение][], [событие][] или [контакт][] в Outlook
- Присутствие [пользователя][] в Microsoft Teams
- [Пользователь][] или [группа][] в Azure Active Directory
- Принтер [в][] службе печати (когда задание печати для принтера попадает в состояние JobFetchable — готово к извлечению для печати).
- [PrintTaskDefinition в][] службе печати
- A [todoTask] of a user in Microsoft To Do

Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Обновив подписку, обновив срок ее действия. |
| [Перечисление подписок](../api/subscription-list.md) | [subscription](subscription.md) | Перечисление активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойств и связей объекта подписки. |
| [Удаление подписки](../api/subscription-delete.md) | Нет | Удаление объекта подписки. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | string | Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми. Обязательный. <br><br>Примечание. Уведомления об изменении корневых элементов диска и списков поддерживают только changeType `updated`. Уведомления об изменении пользователей и групп поддерживают changeType `updated` и `deleted`. |
| notificationUrl | string | URL-адрес конечной точки, которая получает уведомления об изменениях. Этот URL-адрес должен использовать протокол HTTPS. Обязательный. |
| lifecycleNotificationUrl | string | URL-адрес конечной точки, которая получает уведомления жизненного цикла, включая `subscriptionRemoved` и `missed` уведомления. Этот URL-адрес должен использовать протокол HTTPS. Необязательное свойство. <br><br>[Узнайте больше](/graph/webhooks-lifecycle) об использовании уведомлений жизненного цикла в ресурсах Outlook. |
| resource | string | Указывает ресурс, для которого будут отслеживаться изменения. Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`). См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов. Обязательный. |
| expirationDateTime | DateTimeOffset | Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.  В приведенной ниже таблице указан максимально допустимый период подписки. Обязательный. |
| clientState | string | Указывает значение свойства **clientState,** от отправляется службой в каждом уведомлении об изменении. Максимальная длина: 255 символов. Клиент может проверить, поступило ли уведомление об изменении из службы, сравнив значение свойства **clientState,** отправленного с подпиской, со значением свойства **clientState,** полученного с каждым уведомлением об изменении. Необязательное свойство. |
| id | string | Уникальный идентификатор для подписки. Только для чтения. |
| applicationId | string | Идентификатор приложения, использованного для создания подписки. Только для чтения. |
| creatorId | string | Идентификатор пользователя или субъекта-службы, которые создали подписку. Если приложение использовало делегирование разрешений для создания подписки, в этом поле содержится ИД пользователя, выписав его от имени. Если приложение использовало разрешения приложения, это поле содержит ИД основного приложения-службы, соответствующего приложению. Только для чтения. |
| includeResourceData | Boolean | Если присвоено значение `true`, уведомления об изменениях [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата). Необязательно. | 
| encryptionCertificate | string | Представление в кодировке Base64 сертификата с открытым ключом, используемое для шифрования данных ресурса в уведомлениях об изменениях. Необязательно. Обязательно, если **includeResourceData** имеет значение true. | 
| encryptionCertificateId | string | Предоставляемый приложением настраиваемый идентификатор, помогающий определить сертификат, необходимый для расшифровки данных ресурса. Необязательно. Обязательно, если **includeResourceData** имеет значение true. |
| latestSupportedTlsVersion | Строка | Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**. Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2. Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем. </br></br>Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна. В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`. |

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
| **presence**        | 60 минут (1 час) |
| Принтер  печати | 4230 минут (до 3 дней)    |
| **PrintTaskDefinition** | 4230 минут (до 3 дней)    |
| **todoTask**              | 4230 минут (до 3 дней)    |


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

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string"
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
[todoTask]: ./todotask.md

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


