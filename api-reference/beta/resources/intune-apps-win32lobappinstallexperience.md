---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2470aeac3b92052e801db12d4da7f76113a9c8d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422975"
---
# <a name="win32lobappinstallexperience-resource-type"></a>Тип ресурса win32LobAppInstallExperience

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства интерфейса установки приложения Win32

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения, в котором работает приложение. Возможные значения: `system`, `user`.|
|девицерестартбехавиор|[win32LobAppRestartBehavior](../resources/intune-apps-win32lobapprestartbehavior.md)|Поведение устройства перезапускается. Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.|

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



