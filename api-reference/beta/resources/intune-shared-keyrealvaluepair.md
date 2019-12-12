---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d7bbe482d03990a8056e89bbe7608911c1eff9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955640"
---
# <a name="keyrealvaluepair-resource-type"></a>Тип ресурса Кэйреалвалуепаир

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).


Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Строковый ключ для типа "ключ — значение". Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|
|значение|Двойное с плавающей точкой|Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "<Unknown Primitive Type Edm.Double>"
}
```



