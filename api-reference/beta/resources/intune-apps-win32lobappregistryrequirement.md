---
title: Тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 175896a3b086821e4c36a26b5644d08e503d019d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706221"
---
# <a name="win32lobappregistryrequirement-resource-type"></a>Тип ресурса win32LobAppRegistryRequirement

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства реестра для обнаружения приложения Win32


Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|детектионвалуе|Строка|Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|check32BitOn64System|Логический|Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе|
|Ключевой|Строка|Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)|
|valueName|Строка|Имя значения реестра|
|детектионтипе|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Тип обнаружения данных в реестре. Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```





