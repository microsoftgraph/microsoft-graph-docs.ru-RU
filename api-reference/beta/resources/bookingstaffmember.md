---
title: Тип ресурса bookingStaffMember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 382da1b0710b691a6563a40c03ed62397262911d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884457"
---
# <a name="bookingstaffmember-resource-type"></a>Тип ресурса bookingStaffMember

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет сотрудник, который предоставляет службы в [bookingBusiness](bookingbusiness.md).

Сотрудники могут быть частью клиента Office 355 которых настроен business резервирования, или они могут использовать службы электронной почты от других поставщиков электронной почты.

Когда резервирования встреч, API резервирования рассматривает следующие параметры для определения доступности сотрудника: 

1. По умолчанию режим работы бизнеса (свойство **businessHours** сущности [bookingBusiness](bookingbusiness.md) ) представляет общей доступности сотрудника.
2. Если **useBusinessHours** имеет значение false, сотрудник определенных рабочих часов (свойство**workingHours** сущности **bookingStaffmember** ) представляет общей доступности этого элемента.
3. При **availabilityIsAffectedByPersonalCalendar** имеет значение true, затем API резервирования будет сначала откроете сотрудник общедоступной часов (в соответствии с #1 или #2) и убедитесь доступности часам в личный член персонала календарь перед внесением резервирования.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список сотрудников](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) коллекции | Получите список объектов **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Создание bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) коллекции | Создание нового **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Получите свойства и связи **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[обновление](../api/bookingstaffmember-update.md). | [bookingStaffMember](bookingstaffmember.md)    |Обновление свойств **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Delete](../api/bookingstaffmember-delete.md) | Нет |Удалите сотрудник в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Логический|Значение true означает, что если сотрудник является пользователь Office 365, API резервирования будет проверки доступности сотрудника на свой личный календарь в Office 365 перед внесением резервирования. |
|ColorIndex (en)|Int32|Определяет цвет сотрудника. Цвет соответствует цветовой палитры на странице **сведений о персонала** в приложении резервирования.|
|displayName|Строка|Имя сотрудника, как оно отображается для клиентов. Обязательный.|
|emailAddress|String|Адрес электронной почты сотрудника. Это может быть в одном клиентов Office 365 как предприятию или в домене различных электронной почты. Можно использовать этот адрес электронной почты, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса. Обязательный.|
|id|Строка| Идентификатор сотрудника в формате GUID. Только для чтения.|
|role|string| Роль сотрудника в организации. Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`. Обязательный.|
|useBusinessHours|Логический|Имеет значение true означает, что сотрудник доступность — как указанных в свойстве **businessHours** бизнеса. False означает, что доступность определяется значение свойства **workingHours** сотрудника.|
|workingHours|[bookingWorkHours](bookingworkhours.md) коллекции|Диапазон часов каждый день недели, по которым сотрудник доступна для резервирования. По умолчанию они инициализируются совпадает со значением свойства **businessHours** бизнеса.|

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
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
