---
title: тип ресурса win32LobAppInstallExperience
description: Содержит свойства работы с установкой для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a1f844683368d898be7a3acdc1dacbcaffa99ff
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760302"
---
# <a name="win32lobappinstallexperience-resource-type"></a>тип ресурса win32LobAppInstallExperience

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства работы с установкой для приложения Win32

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|Указывает тип контекста выполнения, в котором выполняется приложение. Возможные значения: `system`, `user`.|
|deviceRestartBehavior|[win32LobAppRestartBehavior](../resources/intune-apps-win32lobapprestartbehavior.md)|Поведение перезагрузки устройства. Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```




