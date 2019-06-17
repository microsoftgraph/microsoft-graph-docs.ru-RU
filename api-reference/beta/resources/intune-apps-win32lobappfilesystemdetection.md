---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 447195064a9d42db9756c71dfe08e333bf567b31
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993181"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>Тип ресурса win32LobAppFileSystemDetection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит путь к файлу или папке для обнаружения приложения Win32


Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|path|String|Путь к файлу или папке для определения бизнес-приложения Win32|
|Филеорфолдернаме|String|Имя файла или папки для определения бизнес-приложения Win32|
|check32BitOn64System|Boolean|Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе|
|Детектионтипе|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|Тип обнаружения файловой системы. Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор для обнаружения файлов или папок. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|Детектионвалуе|String|Значение обнаружения файлов или папок|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





