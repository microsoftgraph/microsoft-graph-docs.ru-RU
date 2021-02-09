---
title: Тип ресурса androidDeviceOwnerKioskModeApp
description: Приложение на управляемом домашнем экране владельца устройства Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6adb416c8fd20406c295e56a5d15177e625c30
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161028"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a>Тип ресурса androidDeviceOwnerKioskModeApp

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Приложение на управляемом домашнем экране владельца устройства Android


Наследуется [от androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|package|String|Имя пакета приложения|
|className|String|Имя класса приложения|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```




