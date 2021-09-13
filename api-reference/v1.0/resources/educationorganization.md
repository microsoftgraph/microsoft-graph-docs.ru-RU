---
title: тип ресурса educationOrganization
description: Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 047522db1552f6b48e21868235e3740abe7e6643
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123701"
---
# <a name="educationorganization-resource-type"></a>тип ресурса educationOrganization

Пространство имен: microsoft.graph

Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.

Наследует от [объекта](../resources/entity.md).

## <a name="properties"></a>Свойства

| Свойство             | Тип                    | Описание                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | String                  | Описание организации.                                                              |
| displayName          | Строка                  | Имя отображения организации.                                                             |
| externalSource       | educationExternalSource | Источник, из которых была создана эта организация. Возможные значения: `sis`, `manual`. |
| externalSourceDetail | String                  | Имя внешнего источника, из которого были созданы эти ресурсы.                     |
| id                   | String                  | Идентификатор объекта. Унаследованный от [сущности](../resources/entity.md)                     |

## <a name="relationships"></a>Отношения

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
