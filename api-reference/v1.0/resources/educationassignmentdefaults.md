---
title: Тип ресурса educationAssignmentDefaults
description: Задает значения по умолчанию на уровне класса, которые учитываются новыми назначениями, созданными в классе.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 041cdef8dcdd81493882a7940d0505de94ad16eb
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684685"
---
# <a name="educationassignmentdefaults-resource-type"></a>Тип ресурса educationAssignmentDefaults

Пространство имен: microsoft.graph

Задает значения по умолчанию на уровне класса, которые учитываются новыми назначениями, созданными в классе. 

Вызывающие объекты могут по-прежнему указывать пользовательские значения при каждом создании назначения, если им не нужны поведения по умолчанию.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Чтение свойств и связей объекта [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) .|
|[Обновление educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Обновление свойств объекта [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для educationAssignmentDefaults|
|addedStudentAction|educationAddedStudentAction|Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации задания. Возможные значения: `none`, `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Необязательное поле для управления добавлением заданий в календари учащихся и преподавателей при публикации задания. Возможные значения: , , , `studentsAndTeamOwners`, и . `unknownFutureValue``studentsOnly``studentsAndPublisher``none` Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующих значений в этом развиваемом перечислении необходимо использовать заголовок [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). `studentsOnly` Значение по умолчанию — `none`.|
|dueTime|TimeOfDay|Значение по умолчанию уровня класса для поля времени выполнения. Значение по умолчанию — `23:59:00`.|
|notificationChannelUrl|String|По Teams канал, в который будут отправляться уведомления. Значение по умолчанию — `null`.|

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
  "id": "String (identifier)",
  "addedStudentAction": "String",
  "addToCalendarAction": "educationAddToCalendarOptions",  
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

