---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
ms.openlocfilehash: 7958266fe208e0a04bc72ab658291c58455c763b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322563"
---
# <a name="vpplicensingtype-resource-type"></a>Тип ресурса vppLicensingType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|supportsUserLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования пользователя.|
|supportsDeviceLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования устройства.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



