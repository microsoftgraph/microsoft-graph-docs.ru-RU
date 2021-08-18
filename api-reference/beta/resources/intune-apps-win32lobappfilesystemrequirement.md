---
title: тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь файла или папки для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9f563e4c64528dee49e1aa0a23d417298ec3ece3c1b07df096966a8c5b66fd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240066"
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
|detectionValue|String|Значение обнаружения, унаследованные от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|path|String|Путь файла или папки для обнаружения приложения Win32 Line of Business (LoB)|
|fileOrFolderName|String|Имя файла или папки для обнаружения приложения Win32 Line of Business (LoB)|
|check32BitOn64System|Логический|Значение, указывающее, является ли этот файл или папка для проверки 32-битного приложения в 64-битной системе|
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




