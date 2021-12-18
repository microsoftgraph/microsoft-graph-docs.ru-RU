---
title: тип ресурса educationAssignmentDefaults
description: Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 620798d001df51bff352bcca4dce891a76f22cea
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567393"
---
# <a name="educationassignmentdefaults-resource-type"></a>тип ресурса educationAssignmentDefaults

Пространство имен: microsoft.graph

Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе. 

Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|
|[Обновление educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации назначения. Возможные значения: `none`, `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Необязательное поле для управления добавлением назначений в календари учащихся и преподавателей при публикации. Возможные значения: `none` `studentsAndPublisher` , , , , `studentsAndTeamOwners` и `unknownFutureValue` `studentsOnly` . Обратите внимание, что вы должны использовать загон запроса, чтобы получить следующее значение `Prefer: include-unknown-enum-members` (ы) в этом [развиваемом переуме:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `studentsOnly` . Значение по умолчанию — `none`.|
|dueTime|TimeOfDay|Значение по умолчанию класса для должного поля времени. Значение по умолчанию — `23:59:00`.|
|notificationChannelUrl|Строка|По умолчанию Teams канал, в который будут отправлены уведомления. Значение по умолчанию — `null`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "String",
  "addToCalendarAction": "educationAddToCalendarOptions",  
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

