---
title: тип ресурса keyRealValuePair
description: Пара значения ключа со строкой и реальным (плавающей точкой) значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 66c88b3ec9576f2c18dbcb6c697fed6e2b78474c6e0ee2c7e10f0e4a0d49820f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54203010"
---
# <a name="keyrealvaluepair-resource-type"></a>тип ресурса keyRealValuePair

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пара значения ключа со строкой и реальным (плавающей точкой) значением.


Наследует [от keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|Строка|Клавиша строки пары ключ-значение. Унаследованный от [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|значение|Двойное с плавающей точкой|Значение реального (плавающей точки) пары ключ-значение.|

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
  "value": "4.2"
}
```




