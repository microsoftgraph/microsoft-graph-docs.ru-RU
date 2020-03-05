---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff94d7ddbec70b40b59dc4b1dbfc1b4a5985be3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491017"
---
# <a name="vpplicensingtype-resource-type"></a>Тип ресурса vppLicensingType

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для корпоративного лицензирования приложений iOS (VPP).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|суппортусерлиценсинг|Логический|Указывает, поддерживает ли программа тип лицензирования пользователя.|
|суппортдевицелиценсинг|Boolean|Указывает, поддерживает ли программа тип лицензирования устройства.|
|supportsUserLicensing|Логический|Указывает, поддерживает ли программа тип лицензирования пользователя.|
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
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



