---
title: тип ресурса mobileAppInstallTimeSettings
description: Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b22ae3e5e9b94527417f671d0c6ca3a3545fee6e6819ef31743d0be410129e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251129"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>тип ресурса mobileAppInstallTimeSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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




