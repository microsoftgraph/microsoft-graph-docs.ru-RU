---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c249a21075a2d2647fbb0cbcc53bf7c541a155f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534481"
---
# <a name="win32lobappregistrydetection-resource-type"></a>Тип ресурса win32LobAppRegistryDetection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства реестра для обнаружения приложения Win32


НаСледуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|check32BitOn64System|Логический|Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе|
|Ключевой|String|Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)|
|valueName|String|Имя значения реестра|
|Детектионтипе|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Тип обнаружения данных в реестре. Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор для обнаружения данных в реестре. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|Детектионвалуе|String|Значение обнаружения в реестре|

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





