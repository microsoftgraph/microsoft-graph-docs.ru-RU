---
title: тип ресурса printSettings
description: Представляет параметры для службы универсальной печати для клиента.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4174f6f8dbd1a94ce3246189683529a9fdb4346927465b3f084fb77974313992
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163756"
---
# <a name="printsettings-resource-type"></a>тип ресурса printSettings

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет параметры для службы универсальной печати для клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|documentConversionEnabled|Логический|Указывает, включено ли преобразование документов для клиента. Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (xps to pdf) при необходимости.|

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

