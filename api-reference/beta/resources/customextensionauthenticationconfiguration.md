---
title: тип ресурса customExtensionAuthenticationConfiguration
description: Абстрактный базовый тип, который предоставляет конфигурацию свойства **authenticationConfiguration** производных типов, унаследованных от настраиваемого абстрактного типаCalloutExtension
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3fbe85e5cca096ad0af24b7d0ffa04e035be63a9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339050"
---
# <a name="customextensionauthenticationconfiguration-resource-type"></a>тип ресурса customExtensionAuthenticationConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый тип, который предоставляет конфигурацию для свойства **authenticationConfiguration** производных типов, унаследованных от настраиваемого абстрактного [типаCalloutExtension](customcalloutextension.md) . Этот абстрактный тип наследуется типом [ресурсов azureAdTokenAuthentication](../resources/azureadtokenauthentication.md) .

## <a name="properties"></a>Свойства

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration",
  "abstract": true
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionAuthenticationConfiguration " 
} 
```