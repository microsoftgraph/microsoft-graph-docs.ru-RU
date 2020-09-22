---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a540d862a88168f1e1c195a87f289f520c0b6fed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049249"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Тип ресурса Унсуппортеддевицеконфигуратиондетаил

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описание причин неподдерживаемого объекта.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|message|String|Сообщение с объяснением, почему объект не поддерживается.|
|propertyName|Строка|Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```






