---
title: тип ресурса keyIntegerValuePair
description: Пара значений ключа с ключом строки и компонентным значением.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ecabcb6f4704dc64dddfdb46dc6d26b48e16d05
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131303"
---
# <a name="keyintegervaluepair-resource-type"></a>тип ресурса keyIntegerValuePair

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пара значений ключа с ключом строки и компонентным значением.


Наследует [от keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|key|String|Клавиша строки пары ключ-значение. Унаследованный от [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|value|Int32|Integer value of the key-value pair.|

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



