---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a37d4b6b9e30bc7f0d61bbe3fa92bf6c51ff3547
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216821"
---
# <a name="subscription-resource-type"></a>Тип ресурса subscription

Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.

- [Сообщение][], [событие][] или [контакт][] в Outlook
- [Беседа][] группы Office 365
- Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.
- [Пользователь][] или [группа][] в Azure Active Directory
- [Оповещение][] из Microsoft Graph Security API

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | string | Обязательное. Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.<br><br>Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType. Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.|
| notificationUrl | string | Обязательное. URL-адрес конечной точки, которая будет получать уведомления. Этот URL-адрес должен использовать протокол HTTPS. |
| resource | string | Обязательное. Указывает ресурс, для которого будут отслеживаться изменения. Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Обязательное. Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.  В приведенной ниже таблице указан максимально допустимый период подписки. |
| clientState | string | Необязательно. Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении. Максимальная длина составляет 128 символов. Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением. |
| id | string | Уникальный идентификатор для подписки. Только для чтения. |
| applicationId | string | Идентификатор приложения, использованного для создания подписки. Только для чтения. |
| creatorId | string | Идентификатор пользователя или субъекта-службы, которые создали подписку. Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение. Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению. Только для чтения. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Максимальный период подписки для каждого из типов ресурсов

| Ресурс            | Максимальный срок действия  |
|:--------------------|:-------------------------|
| Пользователь, группа, другие ресурсы каталога   | 4230 минут (до 3 дней)    |
| Почта                | 4230 минут (до 3 дней)    |
| Календарь            | 4230 минут (до 3 дней)    |
| Контакты            | 4230 минут (до 3 дней)    |
| Беседы группы | 4230 минут (до 3 дней)    |
| Элементы в корне диска    | 4230 минут (до 3 дней)    |
| Оповещения системы безопасности     | 43200 минут (до 30 дней)  |

> **Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение. В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.

## <a name="relationships"></a>Отношения

Нет

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Обновление подписки путем изменения ее срока действия. |
| [Перечисление подписок](../api/subscription-list.md) | [subscription](subscription.md) | Перечисление активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойств и связей объекта subscription. |
| [Удаление подписки](../api/subscription-delete.md) | Нет |Удаление объекта subscription. |

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
