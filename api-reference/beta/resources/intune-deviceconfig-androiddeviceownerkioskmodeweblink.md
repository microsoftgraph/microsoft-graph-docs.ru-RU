---
title: Тип ресурса androidDeviceOwnerKioskModeWeblink
description: Веб-связь на управляемом домашнем экране владельца устройства Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 076e1fc6630856ff937bf85396c70e4461fda2b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162555"
---
# <a name="androiddeviceownerkioskmodeweblink-resource-type"></a>Тип ресурса androidDeviceOwnerKioskModeWeblink

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Веб-связь на управляемом домашнем экране владельца устройства Android


Наследуется [от androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Отображаемая имя для веб-ссылки|
|ссылка|String|Ссылка для веб-ссылки|

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




