---
title: тип ресурса printSettings
description: Представляет параметры для службы универсальной печати для клиента.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 11cba611772065f8c2014143f0c83b45eb6bd766
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944265"
---
# <a name="printsettings-resource-type"></a>тип ресурса printSettings

Пространство имен: microsoft.graph

Представляет параметры для службы универсальной печати для клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|documentConversionEnabled|Логическое|Указывает, включено ли преобразование документов для клиента. Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (xps to pdf) при необходимости.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

