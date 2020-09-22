---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 468afea165645c2fc6a728e5a171b1ef37e9e338
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080167"
---
# <a name="win32lobappinstallexperience-resource-type"></a>Тип ресурса win32LobAppInstallExperience

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства интерфейса установки приложения Win32

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
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
  "deviceRestartBehavior": "String"
}
```





