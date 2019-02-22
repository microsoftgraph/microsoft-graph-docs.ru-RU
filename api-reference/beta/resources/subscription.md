---
title: Тип ресурса Subscription
description: 'Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. В настоящее время подписки включены для следующих ресурсов:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163940"
---
# <a name="subscription-resource-type"></a>Тип ресурса Subscription

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. В настоящее время подписки включены для следующих ресурсов:

- [Сообщение][], [событие][]или [контакт][] в Outlook
- [Беседа][] с группой Office 365
- Контент в иерархии корневой папки [driveItem][] в Onedrive для бизнеса или корневой папки или вложенной папки [driveItem][] в личном OneDrive пользователя
- [Пользователь][] или [Группа][] в Azure Active Directory
- [Оповещение][] из API безопасности Microsoft Graph


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | строка | Обязательный. Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми. <br><br>Note: уведомления корневого элемента диска поддерживают только `updated` ChangeType. Поддержка `updated` и `deleted` ChangeType уведомлений для пользователей и групп. |
| notificationUrl | string | Обязательный. URL-адрес конечной точки, которая будет получать уведомления. Этот URL-адрес должен использовать протокол HTTPS. |
| resource | string | Обязательный. Указывает ресурс, для которого будет выполняться отслеживание изменений. Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`). |
| expirationDateTime | DateTimeOffset | Обязательно указывать. Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.  В приведенной ниже таблице указан максимально допустимый период подписки. |
| clientState | string | Необязательный параметр. Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении. Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением. |
| id | string | Уникальный идентификатор для подписки. Только для чтения. |
| applicationId | string | Идентификатор приложения, используемого для создания подписки. Только для чтения. |
| creatorId | string | Идентификатор пользователя или участника службы, который создал подписку. Если приложение использовало делегированные разрешения для создания подписки, это поле содержит идентификатор пользователя, выполнившего вход в систему, вызываемую приложением от имени. Если приложение использовало разрешения приложения, это поле содержит идентификатор участника службы, соответствующего приложению. Только для чтения. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Максимальный период подписки для каждого из типов ресурсов

| Ресурс            | Максимальный срок действия  |
|:--------------------|:-------------------------|
| Почта                | 4230 минут (в течение 3 дней)    |
| Календарь            | 4230 минут (в течение 3 дней)    |
| Контакты            | 4230 минут (в течение 3 дней)    |
| Беседы группы | 4230 минут (в течение 3 дней)    |
| Элементы в корне диска    | 4230 минут (в течение 3 дней)    |
| Оповещения системы безопасности     | 43200 минут (30 дней)  |

> **Примечание:** Существующие приложения и новые приложения не должны превышать поддерживаемое значение. В будущем все запросы на создание или продление подписки, превышающие максимальное значение, завершатся неудачей.

## <a name="relationships"></a>Отношения

Нет

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Продлить подписку, обновив срок ее действия. |
| [Список подписок](../api/subscription-list.md) | [subscription](subscription.md) | Список активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойств и связей объекта Subscription. |
| [Удаление подписки](../api/subscription-delete.md) | Нет | Удаление объекта подписки. |

[контакт]: ./contact.md
[беседа]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[акций]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
