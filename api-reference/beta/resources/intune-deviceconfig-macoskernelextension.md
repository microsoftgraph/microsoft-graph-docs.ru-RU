---
title: тип ресурса macOSKernelExtension
description: Представляет определенное расширение ядра macOS. Расширение ядра macOS можно описать идентификатором группы и идентификатором пакета.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f430f83dbd166ee93f9e0ebfc4baa4ddb9f39db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095572"
---
# <a name="macoskernelextension-resource-type"></a>тип ресурса macOSKernelExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет определенное расширение ядра macOS. Расширение ядра macOS можно описать идентификатором группы и идентификатором пакета.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamIdentifier|String|Идентификатор группы, который использовался для подписи расширения ядра.|
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



