---
title: Тип ресурса educationAssignmentSettings
description: Указывает параметры назначений на уровне класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c670cb2bbef0b82ff80996e4acb52c2826ec118f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034359"
---
# <a name="educationassignmentsettings-resource-type"></a>Тип ресурса educationAssignmentSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметры назначений на уровне класса.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Чтение свойств и связей объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)|
|[Обновление educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|submissionAnimationDisabled|Логический|Указывает, будет ли показана анимация поозднения. Значение `true` указывает, что анимация не будет показана. Значение по умолчанию: `false`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

