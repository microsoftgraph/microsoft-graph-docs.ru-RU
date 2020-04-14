---
title: Тип ресурса Макоскернелекстенсион
description: Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 457d13b2f3f78b52457afd7c30bf3b0e36ca4e92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447054"
---
# <a name="macoskernelextension-resource-type"></a>Тип ресурса Макоскернелекстенсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|теамидентифиер|String|Идентификатор команды, использованный для подписи расширения ядра.|
|bundleId|String|Идентификатор пакета расширения ядра.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



