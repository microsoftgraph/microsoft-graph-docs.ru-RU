---
title: тип ресурса educationAssignmentDefaults
description: Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cdd4cb3814900f41f7cb7ee5ede407af61e9c4d7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781067"
---
# <a name="educationassignmentdefaults-resource-type"></a>тип ресурса educationAssignmentDefaults

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе. Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|
|[Обновление educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации назначения. Возможные значения: `none`, `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Необязательное поле для управления asfor добавлением назначений в календари учащихся и преподавателей при публикации задания. Возможные значения: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`. Значение по умолчанию — `none`.|
|dueTime|TimeOfDay|Значение по умолчанию класса для должного поля времени. Значение по умолчанию — `23:59:00`.|
|notificationChannelUrl|String|По умолчанию Teams канал, в который будут отправлены уведомления. Значение по умолчанию — `null`.|

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
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

