---
title: тип ресурса educationOrganization
description: Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24313b6b6061449faea0ecb4880a421a2333099
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231866"
---
# <a name="educationorganization-resource-type"></a>тип ресурса educationOrganization

Пространство имен: microsoft.graph

Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.

Наследует от [объекта](../resources/entity.md).

## <a name="properties"></a>Свойства

| Свойство             | Тип                    | Описание                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | Строка                  | Описание организации.                                                              |
| displayName          | Строка                  | Имя отображения организации.                                                             |
| externalSource       | educationExternalSource | Источник, из которых была создана эта организация. Возможные значения: `sis`, `manual`. |
| externalSourceDetail | Строка                  | Имя внешнего источника, из которого были созданы эти ресурсы.                     |
| id                   | Строка                  | Идентификатор объекта. Унаследованный от [сущности](../resources/entity.md)                     |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
