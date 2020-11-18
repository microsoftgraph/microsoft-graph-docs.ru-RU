---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 619c925ff58745054a4cc62c638f1776ee96d5f2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199016"
---
# <a name="edgesearchengine-resource-type"></a>Тип ресурса edgeSearchEngine

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




