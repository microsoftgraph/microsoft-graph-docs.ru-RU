---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fbd54fe4ed8f7df35ae6acdcde8722b98d1c24a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335552"
---
# <a name="win32lobappregistrydetection-resource-type"></a>Тип ресурса win32LobAppRegistryDetection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства реестра для обнаружения приложения Win32


Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|check32BitOn64System|Boolean|Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе|
|Ключевой|String|Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)|
|valueName|String|Имя значения реестра|
|детектионтипе|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Тип обнаружения данных в реестре. Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор для обнаружения данных в реестре. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|детектионвалуе|String|Значение обнаружения в реестре|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



