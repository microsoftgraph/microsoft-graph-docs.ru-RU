---
title: тип ресурса educationAssignmentSettings
description: Указывает параметры назначений на уровне класса.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c920db8b8d3b6ea8a3c49e4a4816740d59a8e534aa542a1a906451654eaf7f6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212121"
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
|submissionAnimationDisabled|Логическое|Указывает, будет ли показана анимация празднования по очереди. Значение `true` указывает, что анимация не будет показана. Значение по умолчанию — `false`.|

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

