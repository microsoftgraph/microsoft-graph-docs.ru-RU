---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8dc3185493501436f8cd7d7722379b09287e4dad
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924551"
---
# <a name="keyintegervaluepair-resource-type"></a>Тип ресурса Кэйинтежервалуепаир

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение типа "ключ — значение" с ключом строки и целым значением.


Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Строковый ключ для типа "ключ — значение". Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|
|value|Int32|Целочисленное значение для параметра "ключ — значение".|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyIntegerValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyIntegerValuePair",
  "key": "String",
  "value": 1024
}
```



