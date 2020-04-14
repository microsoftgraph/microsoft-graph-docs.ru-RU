---
title: Тип ресурса Букингстаффмембер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 055627af88a51c73d81d23c8ccd1a6e1f4af5d45
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43360544"
---
# <a name="bookingstaffmember-resource-type"></a>Тип ресурса Букингстаффмембер

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сотрудника, который предоставляет службы в [букингбусинесс](bookingbusiness.md).

Сотрудники могут входить в состав клиента Office 355, на котором настроена Настройка бизнеса, или они могут использовать службы электронной почты от других поставщиков услуг электронной почты.

При резервировании встреч API учета рассматривает следующие параметры для определения доступности сотрудников: 

1. По умолчанию часы работы бизнеса (свойство **businessHours** объекта [букингбусинесс](bookingbusiness.md) ) представляют общую доступность сотрудника.
2. Если **усебусинесшаурс** имеет значение false, то характер рабочего времени сотрудника (свойства**воркингхаурс** объекта **букингстаффмембер** ) представляет общую доступность этого члена.
3. Если **аваилабилитисаффектедбиперсоналкалендар** имеет значение true, то API для резервирования будет сначала просматривать доступные часы сотрудника (как определено #1, так #2), а также проверять доступность в течение этих часов в личном календаре сотрудника перед выполнением резервирования.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список сотрудников](../api/bookingbusiness-list-staffmembers.md) | Коллекция [букингстаффмембер](bookingstaffmember.md) | Получение списка объектов **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md). |
|[Создание Букингстафф](../api/bookingbusiness-post-staffmembers.md) | Коллекция [букингстаффмембер](bookingstaffmember.md) | Создание нового **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md). |
|[Получение Букингстаффмембер](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Получение свойств и связей объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).|
|[обновление](../api/bookingstaffmember-update.md). | [bookingStaffMember](bookingstaffmember.md)    |Обновление свойств объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).|
|[удаление](../api/bookingstaffmember-delete.md); | Нет |Удаление сотрудника в заданном [букингбусинесс](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|аваилабилитисаффектедбиперсоналкалендар|Логическое|True означает, что если сотрудник является пользователем Office 365, то API для резервирования будет проверять доступность сотрудников в личном календаре в Office 365 перед выполнением резервирования. |
|colorIndex|Int32|Определяет цвет для представления сотрудника. Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".|
|displayName|Строка|Имя сотрудника, отображаемое для клиентов. Обязательно.|
|emailAddress|String|Адрес электронной почты сотрудника. Это может быть тот же клиент Office 365, что и в Организации, или в другом домене электронной почты. Этот адрес электронной почты можно использовать, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true. Обязательный.|
|id|String| Идентификатор сотрудника в формате GUID. Только для чтения.|
|role|string| Роль сотрудника в Организации. Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`. Обязательно.|
|усебусинесшаурс|Логическое|Значение true означает, что уровень доступности сотрудника указан в свойстве **businessHours** предприятия. Значение false означает, что доступность определяется значением свойства **воркингхаурс** сотрудника.|
|workingHours|Коллекция [букингворкхаурс](bookingworkhours.md)|Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования. По умолчанию они инициализируются так же, как свойство **businessHours** для бизнеса.|

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
