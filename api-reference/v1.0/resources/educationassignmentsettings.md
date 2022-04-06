---
title: Тип ресурса educationAssignmentSettings
description: Задает параметры назначений на уровне класса.
author: sharad-sharma-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2421aabe7089e140b4cb9997b1d0143ed8e9f234
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684678"
---
# <a name="educationassignmentsettings-resource-type"></a>Тип ресурса educationAssignmentSettings

Пространство имен: microsoft.graph

Задает параметры назначений на уровне класса.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Чтение свойств и связей объекта [educationAssignmentSettings](../resources/educationassignmentsettings.md) .|
|[Обновление educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Обновление свойств объекта [educationAssignmentSettings](../resources/educationassignmentsettings.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта educationAssignmentSettings.|
|submissionAnimationDisabled|Логический|Указывает, будет ли отображаться анимация с пошаговой анимацией. Значение указывает, `true` что анимация не будет отображаться. Значение по умолчанию — `false`.|

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
  "id": "String (identifier)",
  "submissionAnimationDisabled": false
}
```

