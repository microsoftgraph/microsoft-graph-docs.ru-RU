---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7c62ec2cf1fbe5a78534bdb5f6ff9b1e73e37c9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924523"
---
# <a name="keystringvaluepair-resource-type"></a>Тип ресурса Кэйстрингвалуепаир

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение типа "ключ — значение" со строковым ключом и строковым значением.


Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Строковый ключ для типа "ключ — значение". Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|
|value|String|Строковое значение для параметра "ключ — значение".|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



