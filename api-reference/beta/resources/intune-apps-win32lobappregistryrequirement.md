---
title: тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79635640146382baf77aec3858f0dffacfd5ec5f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787885"
---
# <a name="win32lobappregistryrequirement-resource-type"></a>тип ресурса win32LobAppRegistryRequirement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства реестра для обнаружения приложения Win32


Наследует [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор обнаружения, унаследованный от [win32LobAppRequirement.](../resources/intune-apps-win32lobapprequirement.md) Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Строка|Значение обнаружения, унаследованные от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|check32BitOn64System|Логический|Значение, указывающее, является ли этот путь реестра для проверки 32-битного приложения в 64-битной системе|
|keyPath|Строка|Путь ключа реестра для обнаружения приложения Win32 Line of Business (LoB)|
|valueName|Строка|Имя значения реестра|
|detectionType|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Тип обнаружения данных реестра. Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|

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



