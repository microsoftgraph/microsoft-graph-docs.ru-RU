---
title: Тип ресурса Subscription
description: 'Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены следующие ресурсы:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517269"
---
# <a name="subscription-resource-type"></a>Тип ресурса subscription

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены следующие ресурсы:

- Почта, события и контакты из Outlook.
- Беседы в группах Office.
- Корневые элементы диска в OneDrive.
- Пользователи и группы из Azure Active Directory.
- Оповещения о от безопасности Microsoft Graph API.

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
| changeType | строка | Обязательный. Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление. Поддерживаемые значения: `created`, `updated`, `deleted`. Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми. <br><br>Примечание: Диск корневого элемента уведомлений поддерживает только `updated` changeType. Уведомления пользователей и групп поддержки `updated` и `deleted` changeType. |
| notificationUrl | string | Обязательный. URL-адрес конечной точки, который будет получать уведомления. Этот URL-адрес необходимо использовать протокол HTTPS протокола. |
| resource | string | Обязательный. Указывает ресурс, к которому будет выполняться мониторинг изменений. Не включать базовый URL-адрес (`https://graph.microsoft.com/beta/`). |
| expirationDateTime | DateTimeOffset | Обязательный. Указывает дату и время истечения срока действия подписки на веб-перехватчик. Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.  В приведенной ниже таблице указан максимально допустимый период подписки. |
| clientState | string | Необязательный параметр. Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении. Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением. |
| id | string | Уникальный идентификатор для подписки. Только для чтения. |
| applicationId | string | Идентификатор приложения, используемого для создания подписки. Только для чтения. |
| creatorId | string | Идентификатор пользователя или участника-службы, которая создана подписка. Если используется приложение делегированных разрешений на создание подписки, это поле содержит код вызова приложения от имени владельца пользователь выполнил вход. Если приложение разрешения приложения, это поле содержит идентификатор участника-службы, соответствующего приложения. Только для чтения. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Максимальный период подписки для каждого из типов ресурсов

| Ресурс            | Максимальный срок действия  |
|:--------------------|:-------------------------|
| Почта                | 4230 минут (в разделе 3 дня)    |
| Календарь            | 4230 минут (в разделе 3 дня)    |
| Контакты            | 4230 минут (в разделе 3 дня)    |
| Беседы группы | 4230 минут (в разделе 3 дня)    |
| Элементы в корне диска    | 4230 минут (в разделе 3 дня)    |
| Оповещения системы безопасности     | 43200 минут (в разделе 30 дней)  |

> **Примечание:** Поддерживаемые значения не должна превышать существующих приложений и новых приложений. В дальнейшем все запросы, чтобы создать или обновить подписку за пределы максимальное значение завершится с ошибкой.

## <a name="relationships"></a>Отношения

Нет

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
| [Создание подписки](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph. |
| [Обновление подписки](../api/subscription-update.md) | [subscription](subscription.md) | Продление подписки, изменив его время истечения срока действия. |
| [Список подписок](../api/subscription-list.md) | [subscription](subscription.md) | Список активных подписок. |
| [Получение подписки](../api/subscription-get.md) | [subscription](subscription.md) | Чтение свойства и связи объекта подписки. |
| [Удаление подписки](../api/subscription-delete.md) | Нет | Удалите объект подписки. |

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
