---
title: тип ресурса educationOrganization
description: Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fa6d324602ba13ebe186bc0631de991e193d945757117217aa29296ee480ef74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130354"
---
# <a name="educationorganization-resource-type"></a>тип ресурса educationOrganization

Пространство имен: microsoft.graph

Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.

Наследует от [объекта](../resources/entity.md).

## <a name="properties"></a>Свойства

| Свойство             | Тип                    | Описание                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | String                  | Описание организации.                                                              |
| displayName          | String                  | Имя отображения организации.                                                             |
| externalSource       | educationExternalSource | Источник, из которых была создана эта организация. Возможные значения: `sis`, `manual`. |
| externalSourceDetail | String                  | Имя внешнего источника, из которого были созданы эти ресурсы.                     |
| id                   | String                  | Идентификатор объекта. Унаследованный от [сущности](../resources/entity.md)                     |

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
