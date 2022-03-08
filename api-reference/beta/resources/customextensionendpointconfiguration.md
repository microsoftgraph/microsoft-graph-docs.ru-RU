---
title: тип ресурса customExtensionEndpointConfiguration
description: Абстрактный базовый тип, который предоставляет производные типы, используемые для настройки свойства endpointConfiguration объекта расширения рабочего процесса пользовательского пакета доступа.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8607ee8311c0cfc64eef06c3dc2716fb775473fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339617"
---
# <a name="customextensionendpointconfiguration-resource-type"></a>тип ресурса customExtensionEndpointConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый тип, который предоставляет производные типы, используемые для настройки свойства **endpointConfiguration** объекта расширения рабочего процесса пользовательского пакета [доступа](customaccesspackageworkflowextension.md) . Этот абстрактный тип наследуется [объектом logicAppTriggerEndpointConfiguration](logicapptriggerendpointconfiguration.md) .

## <a name="properties"></a>Свойства

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration",
  "abstract": true
}
-->
``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionEndpointConfiguration" 
} 
```