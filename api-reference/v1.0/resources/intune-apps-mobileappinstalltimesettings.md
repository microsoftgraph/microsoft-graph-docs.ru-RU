---
title: тип ресурса mobileAppInstallTimeSettings
description: Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63107dec2435ee0b8cbcda2f13febb18e1a64356
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457633"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>тип ресурса mobileAppInstallTimeSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|useLocalTime|Логический|Следует ли использовать местное время устройства или время UTC при определении доступных и крайних сроков.|
|startDateTime|DateTimeOffset|Время, в которое приложение должно быть доступно для установки.|
|deadlineDateTime|DateTimeOffset|Время установки приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```



