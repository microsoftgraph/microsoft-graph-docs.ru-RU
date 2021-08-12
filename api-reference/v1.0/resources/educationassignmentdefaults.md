---
title: тип ресурса educationAssignmentDefaults
description: Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d9b9b624030129e85b2d89dc05db605af3cae7a4de72d019b41144a9453a23d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230769"
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
  "addedStudentAction": "String",
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

