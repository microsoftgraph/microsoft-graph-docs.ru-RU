---
title: тип ресурса accessPackageResourceAttribute
description: Ресурс, который предоставляет свойства для запрашивателя пакета доступа для предоставления настраиваемой информации, которая может быть использована для принятия решений об утверждении пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9da68399fd09b6277499985fdc87512d7a5c5ae9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861342"
---
# <a name="accesspackageresourceattribute-resource-type"></a>тип ресурса accessPackageResourceAttribute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, который предоставляет свойства для запрашивателя пакета доступа для предоставления настраиваемой информации, которая может быть использована для принятия решений об утверждении пакета доступа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|Сведения о том, как установить атрибут.|
|attributeName|String|Имя атрибута в конечной системе.|
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|Сведения о том, как заполнить значение атрибута при выполнении **accessPackageAssignmentRequest.**|
|id|String|Уникальный идентификатор атрибута.|
|isEditable|String| Указывает, может ли запрашиватель изменить существующее значение атрибута.|
|isPersistedOnAssignmentRemoval|Логический| Указывает, останется ли атрибут в конечном системе после окончания назначения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
}
```
