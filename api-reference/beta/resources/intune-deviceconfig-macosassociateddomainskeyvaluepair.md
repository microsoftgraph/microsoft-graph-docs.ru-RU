---
title: Тип ресурса МакосассоЦиатеддомаинскэйвалуепаир
description: Комбинация "ключ — значение" для связанных доменов
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebf62a01d4a97fde51974ea2e7984b97c39dc5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439724"
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



