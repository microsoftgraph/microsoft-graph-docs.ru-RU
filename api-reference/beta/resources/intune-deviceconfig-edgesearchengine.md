---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a83965eb67762135eba3dcf1edf31fb4aec7827
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946730"
---
# <a name="edgesearchengine-resource-type"></a>Тип ресурса edgeSearchEngine

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.


Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune-deviceconfig-edgesearchenginetype.md)|Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств. Возможные значения: `default`, `bing`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```




