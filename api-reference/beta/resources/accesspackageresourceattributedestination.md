---
title: тип ресурса accessPackageResourceAttributeDestination
description: Абстрактный тип, который предоставляет объекты, определяемые конечными системами, в которые будут переданы настроенные пользователем значения.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7254c0910e930cfcb3d96fd1e4f529a6e9551c3
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468337"
---
# <a name="accesspackageresourceattributedestination-resource-type"></a>тип ресурса accessPackageResourceAttributeDestination

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, используемый для **свойства attributeDestination** [accessPackageResourceAttribute](accesspackageresourceattribute.md). Фактическим назначением будет подтип этого сложного типа.

В настоящее время единственным поддерживаемым подтипом [является accessPackageUserDirectoryAttributeStore](../resources/accesspackageuserdirectoryattributestore.md).  

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeDestination"
}
```
