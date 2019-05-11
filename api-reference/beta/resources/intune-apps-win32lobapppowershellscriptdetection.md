---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 440f86e0056c45f325a9a9bd88f737a91c8efb2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949677"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>Тип ресурса win32LobAppPowerShellScriptDetection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства скрипта PowerShell для обнаружения приложения Win32


Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Свойства enforcesignaturecheck|Логический|Значение, указывающее, применяется ли проверка подписи|
|runAs32Bit|Логический|Значение, указывающее, должен ли этот скрипт выполняться как 32 бит|
|Скриптконтент|Строка|Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




