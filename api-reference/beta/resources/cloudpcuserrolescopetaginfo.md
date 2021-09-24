---
title: тип ресурса cloudPcUserRoleScopeTagInfo
description: Представляет сведения тега области с отображаемой именем и удостоверением.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c070e11bb86b9a41ed5de05955a39599ee21e2f4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507202"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a>тип ресурса cloudPcUserRoleScopeTagInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения тега области с отображаемой именем и удостоверением.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения тегов области.|
|roleScopeTagId|String|ID тега области.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserRoleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```
