---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efba214d6cd6b4e8fb79ddb4df4c9df0e16974bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092547"
---
# <a name="keyintegervaluepair-resource-type"></a>Тип ресурса Кэйинтежервалуепаир

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение типа "ключ — значение" с ключом строки и целым значением.


Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Строковый ключ для типа "ключ — значение". Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)|
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






