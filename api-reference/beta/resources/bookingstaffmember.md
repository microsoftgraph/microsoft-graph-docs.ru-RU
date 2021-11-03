---
title: тип ресурса bookingStaffMember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 4df4584c787c46432a85eb0fcbd61bc11a3531b5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696576"
---
# <a name="bookingstaffmember-resource-type"></a>тип ресурса bookingStaffMember

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сотрудника, который предоставляет услуги в [bookingBusiness.](bookingbusiness.md)

Сотрудники могут быть частью клиента Microsoft 365, где настроен бизнес бронирования, или они могут использовать службы электронной почты от других поставщиков электронной почты.

API бронирования при бронировании рассматривает следующие параметры для определения доступности сотрудника: 

1. По умолчанию часы работы предприятия (свойство **businessHours** объекта [bookingBusiness)](bookingbusiness.md) представляют общую доступность сотрудника.
2. Если **useBusinessHours** является ложным, то конкретные рабочие часы сотрудника (свойство **workingHours** объекта **bookingStaffmember)** представляют общую доступность этого члена.
3. Если **доступностьIsAffectedByPersonalCalendar** верна, то API bookings сначала будет смотреть на общедоступные часы сотрудника (в качестве определенного #1 или #2), а затем проверять доступность в эти часы в личном календаре сотрудника, прежде чем делать заказ.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список сотрудников](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) collection | Получите список объектов **bookingStaffMember** в указанном [bookingbusiness.](../resources/bookingbusiness.md) |
|[Создание bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) collection | Создание нового **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Получить bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Получите свойства и связи **bookingStaffMember** в указанном [bookingbusiness.](../resources/bookingbusiness.md)|
|[Обновление](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |Обновление свойств **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Удаление](../api/bookingstaffmember-delete.md) | Нет |Удаление сотрудника в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Логический|True означает, что если сотрудник является пользователем Microsoft 365, API Bookings проверяет наличие сотрудника в личном календаре в Microsoft 365, прежде чем сделать заказ. |
|colorIndex|Int32|Определяет цвет для представления сотрудника. Цвет соответствует цветовой палитре на странице **Сведения о персонале** в приложении Bookings.|
|displayName|String|Имя сотрудника, отображаемого клиентам. Обязательно.|
|emailAddress|String|Адрес электронной почты сотрудника. Это может быть в том же Microsoft 365 клиенте, что и бизнес, или в другом домене электронной почты. Этот адрес электронной почты можно использовать, если свойство **sendConfirmationsToOwner** заданной в политике планирования бизнеса. Обязательный.|
|id|String| ID сотрудника в формате GUID. Только для чтения.|
|role|string| Роль сотрудника в бизнесе. Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`. Обязательно.|
|timeZone|String|Часовой пояс сотрудника. Список возможных значений см. в [списке dateTimeTimeZone.](datetimetimezone.md)|
|useBusinessHours|Логический|True означает, что доступность сотрудника указана в свойстве **businessHours** бизнеса. False означает, что доступность определяется параметром **свойства workingHours** сотрудника.|
|workingHours|[коллекция bookingWorkHours](bookingworkhours.md)|Диапазон часов, каждый день недели, когда сотрудник доступен для бронирования. По умолчанию они инициализируются так же, как свойство **businessHours** бизнеса.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "timeZone": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


