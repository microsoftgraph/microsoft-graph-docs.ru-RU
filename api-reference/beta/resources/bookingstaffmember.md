---
title: Тип ресурса bookingStaffMember
description: Представляет сотрудника, который предоставляет услуги в bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 25569646633195e9cbce1067dad1abbd369885a2
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160631"
---
# <a name="bookingstaffmember-resource-type"></a>Тип ресурса bookingStaffMember

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сотрудника, который предоставляет услуги в [bookingBusiness](bookingbusiness.md).

Сотрудники могут быть частью клиента Microsoft 365, в котором настроена компания по резервированию, или могут использовать службы электронной почты от других поставщиков услуг электронной почты.

При резервировании встреч API Bookings рассматривает следующие параметры для определения доступности сотрудника: 

1. По умолчанию часы работы предприятия (свойство **businessHours** сущности [bookingBusiness](bookingbusiness.md) ) представляют общую доступность сотрудника.
2. Если **параметр useBusinessHours** имеет значение false, то рабочее время сотрудника (свойство **workingHours** сущности **bookingStaffmember** ) представляет общую доступность этого члена.
3. Если **параметр availabilityIsAffectedByPersonalCalendar** имеет значение true, API Bookings сначала будет проверять общедоступные часы сотрудника (в соответствии с #1 или 2) и проверять доступность в эти часы в личном календаре сотрудника, прежде чем делать резервирование.

Microsoft Bookings поддерживает не более 100 сотрудников в календаре резервирования.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление сотрудников](../api/bookingbusiness-list-staffmembers.md) | [Коллекция bookingStaffMember](bookingstaffmember.md) | Получение списка объектов **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Создание bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [Коллекция bookingStaffMember](bookingstaffmember.md) | Создайте **объект bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Получение свойств и связей **объекта bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Обновление](../api/bookingstaffmember-update.md) | Нет   |Обновите свойства **объекта bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Удаление](../api/bookingstaffmember-delete.md) | Нет |Удаление сотрудника в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True означает, что если сотрудник является Microsoft 365 пользователем, API Bookings проверяет доступность сотрудника в личном календаре в Microsoft 365, прежде чем делать резервирование. |
|colorIndex|Int32|Определяет цвет, представляющий сотрудника. Цвет соответствует цветовой палитре на странице **сведений** о персонале в приложении Bookings.|
|displayName|Строка|Имя сотрудника, отображаемое клиентам. Обязательный элемент.|
|emailAddress|String|Адрес электронной почты сотрудника. Он может быть в том же Microsoft 365, что и бизнес, или в другом домене электронной почты. Этот адрес электронной почты можно использовать, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса. Обязательный.|
|id|Строка| Идентификатор сотрудника в формате GUID. Только для чтения.|
|IsEmailNotificationEnabled|Boolean|`True` означает, что сотрудник будет получать уведомления по электронной почте при создании или изменении назначенного ему резервирования.
|role|bookingStaffRole| Роль сотрудника в организации. Возможные значения: `guest`, , , `viewer`, `externalGuest`, и `scheduler` `unknownFutureValue``member`. `administrator` Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса `[evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`, чтобы получить следующие значения в следующем: `scheduler`, `member`. Обязательный элемент. |
|timeZone|String|Часовой пояс сотрудника. Список возможных значений см. в [разделе dateTimeTimeZone](datetimetimezone.md).|
|useBusinessHours|Boolean|Значение true означает, что доступность сотрудника указана в свойстве **businessHours** компании. Значение false означает, что доступность определяется параметром свойства **workingHours** сотрудника.|
|workingHours|[Коллекция bookingWorkHours](bookingworkhours.md)|Диапазон часов каждый день недели, в течение которого сотрудник доступен для резервирования. По умолчанию они инициализируются так же, как свойство **businessHours** компании.|

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
  "role": {"@odata.type": "microsoft.graph.bookingStaffRole"},
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "timeZone": "String",
  "IsEmailNotificationEnabled": "Boolean"
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


