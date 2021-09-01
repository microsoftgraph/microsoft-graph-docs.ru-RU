---
title: тип ресурса macOSKernelExtension
description: Представляет определенное расширение ядра macOS. Расширение ядра macOS можно описать идентификатором группы и идентификатором пакета.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 281fcab335fc5638c3d376d086bc3d7de6e07aac
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789652"
---
# <a name="macoskernelextension-resource-type"></a>тип ресурса macOSKernelExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет определенное расширение ядра macOS. Расширение ядра macOS можно описать идентификатором группы и идентификатором пакета.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamIdentifier|Строка|Идентификатор группы, который использовался для подписи расширения ядра.|
|bundleId|String|Bundle ID расширения ядра.|

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



