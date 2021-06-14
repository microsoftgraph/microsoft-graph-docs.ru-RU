---
title: тип ресурса educationAssignmentSettings
description: Указывает параметры назначений на уровне класса.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ccaa51c84e50e2f9c5302836ffd9b92754f517fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912937"
---
# <a name="educationassignmentsettings-resource-type"></a>тип ресурса educationAssignmentSettings

Пространство имен: microsoft.graph

Указывает параметры назначений на уровне класса.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)|
|[Обновление educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|submissionAnimationDisabled|Логический|Указывает, будет ли показана анимация празднования по очереди. Значение `true` указывает, что анимация не будет показана. Значение по умолчанию — `false`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

