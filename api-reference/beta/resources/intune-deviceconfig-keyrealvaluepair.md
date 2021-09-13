---
title: тип ресурса keyRealValuePair
description: Пара значения ключа со строкой и реальным (плавающей точкой) значением.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca37d63a8a81a9d66e85890c7ed13b82f30cae15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127208"
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
|key|String|Клавиша строки пары ключ-значение. Унаследованный от [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
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



