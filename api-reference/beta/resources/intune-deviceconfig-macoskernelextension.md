---
title: тип ресурса macOSKernelExtension
description: Представляет определенное расширение ядра macOS. Расширение ядра macOS можно описать идентификатором группы и идентификатором пакета.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb01902173135d20ac1568006c398de88ea8b1061f35681f70c51b5b7dc23ceb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244997"
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




