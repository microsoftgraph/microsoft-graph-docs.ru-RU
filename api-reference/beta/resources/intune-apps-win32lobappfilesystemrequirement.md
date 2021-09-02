---
title: тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь файла или папки для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa212f952f9b4fa87e5916dfbc02de694b6cb030
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790187"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a>тип ресурса win32LobAppFileSystemRequirement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит путь файла или папки для обнаружения приложения Win32


Наследует [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор обнаружения, унаследованный от [win32LobAppRequirement.](../resources/intune-apps-win32lobapprequirement.md) Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Строка|Значение обнаружения, унаследованные от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|path|String|Путь файла или папки для обнаружения приложения Win32 Line of Business (LoB)|
|fileOrFolderName|Строка|Имя файла или папки для обнаружения приложения Win32 Line of Business (LoB)|
|check32BitOn64System|Boolean|Значение, указывающее, является ли этот файл или папка для проверки 32-битного приложения в 64-битной системе|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|Тип обнаружения файловой системы. Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```



