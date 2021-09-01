---
title: тип ресурса androidDeviceOwnerKioskModeManagedFolder
description: Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6144091708f3abfea6aa0f8e0b4ac7284cf58580
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787029"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a>тип ресурса androidDeviceOwnerKioskModeManagedFolder

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|folderName|Строка|Отображение имени папки|
|folderIdentifier|Строка|Уникальный идентификатор для папки|
|элементы|[коллекция androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)|Элементы, которые необходимо добавить в управляемой папке. Эта коллекция может содержать не более 500 элементов.|

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



