---
title: Тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fae649a738416ee4c164da645906467d4cf43a08
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261092"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>Тип ресурса win32LobAppPowerShellScriptRequirement

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства скрипта PowerShell для обнаружения приложения Win32


Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|детектионвалуе|String|Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|displayName|String|Уникальное отображаемое имя для этого правила|
|Свойства enforcesignaturecheck|Boolean|Значение, указывающее, применяется ли проверка подписи|
|runAs32Bit|Boolean|Значение, указывающее, должен ли этот скрипт выполняться как 32 бит|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения, в котором выполняется скрипт. Возможные значения: `system`, `user`.|
|скриптконтент|String|Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32|
|детектионтипе|[win32LobAppPowerShellScriptDetectionType](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|Тип обнаружения для вывода сценария. Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```




