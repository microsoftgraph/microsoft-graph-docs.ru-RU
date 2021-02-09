---
title: Тип ресурса androidDeviceOwnerKioskModeManagedFolder
description: Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6b373729ffebb3fc7a08ee29e98f3471c8c27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162561"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a>Тип ресурса androidDeviceOwnerKioskModeManagedFolder

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|folderName|String|Отображаемая имя папки|
|folderIdentifier|String|Уникальный идентификатор папки|
|items|[Коллекция androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)|Элементы, добавляемые в управлую папку. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```




