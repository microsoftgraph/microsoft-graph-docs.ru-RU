---
title: Тип ресурса МакосассоЦиатеддомаинскэйвалуепаир
description: Комбинация "ключ — значение" для связанных доменов
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc73af5746dce61961563b84871e35bab1982c09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055444"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a>Тип ресурса МакосассоЦиатеддомаинскэйвалуепаир

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Комбинация "ключ — значение" для связанных доменов


Наследуется от [KeyValuePair](../resources/intune-shared-keyvaluepair.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя для этой ключевой [РазkeyValuePairа](../resources/intune-shared-keyvaluepair.md) , унаследованной от|
|value|String|Значение для этой заданной для этой основе ключа, унаследованной от [KeyValuePair](../resources/intune-shared-keyvaluepair.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```






