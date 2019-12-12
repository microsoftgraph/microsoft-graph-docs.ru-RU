---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4498f107e3153f6809ceb664c07b3f53a8d8e0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955647"
---
# <a name="keybooleanvaluepair-resource-type"></a>Тип ресурса Кэйбулеанвалуепаир

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение типа "ключ — значение" с ключом строки и логическим значением.


Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Строковый ключ для типа "ключ — значение". Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|
|value|Boolean|Логическое значение для параметра "ключ — значение".|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyBooleanValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyBooleanValuePair",
  "key": "String",
  "value": true
}
```



