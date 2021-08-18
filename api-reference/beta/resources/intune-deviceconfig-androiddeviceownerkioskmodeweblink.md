---
title: тип ресурса androidDeviceOwnerKioskModeWeblink
description: Веб-ссылки на управляемом домашнем экране владельца android-устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 93e045762474c98204e022b7ea3329ee344e16c95986415a6e6410737c82c6a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236495"
---
# <a name="androiddeviceownerkioskmodeweblink-resource-type"></a>тип ресурса androidDeviceOwnerKioskModeWeblink

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Веб-ссылки на управляемом домашнем экране владельца android-устройств


Наследует [от androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|String|Отображение имени веб-ссылки|
|link|Строка|Ссылка для веб-ссылки|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeWeblink",
  "label": "String",
  "link": "String"
}
```




