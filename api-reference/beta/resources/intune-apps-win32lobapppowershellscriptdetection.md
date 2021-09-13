---
title: тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c611f83d591805a7f728989edcd222f5ea690146
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111385"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>тип ресурса win32LobAppPowerShellScriptDetection

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства скрипта PowerShell для обнаружения приложения Win32


Наследует [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enforceSignatureCheck|Логический|Значение, указывающее, выполняется ли проверка подписи|
|runAs32Bit|Логический|Значение, указывающее, должен ли этот скрипт работать как 32-битный|
|scriptContent|String|Кодированное содержимое скрипта base64 для обнаружения приложения Win32 Line of Business (LoB)|

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



