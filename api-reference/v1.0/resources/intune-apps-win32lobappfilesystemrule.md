---
title: тип ресурса win32LobAppFileSystemRule
description: Сложный тип для хранения данных правил файлов или папок для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fef9a20c7a5bf8c9dd493e3fe5aa9b24e567a793
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60456546"
---
# <a name="win32lobappfilesystemrule-resource-type"></a>тип ресурса win32LobAppFileSystemRule

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения данных правил файлов или папок для приложения LOB Win32.


Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий цель правила. Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|path|String|Путь к файлу или папке.|
|fileOrFolderName|String|Имя файла или папки.|
|check32BitOn64System|Логический|Значение, указывающее, следует ли расширять переменные среды в 32-битной среде на 64-битных системах.|
|operationType|[win32LobAppFileSystemOperationType](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|Тип операции файловой системы. Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор обнаружения файлов или папок. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|String|Значение сравнения файла или папки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRule",
  "ruleType": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```



