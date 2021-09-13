---
title: тип ресурса androidDeviceOwnerKioskModeManagedFolder
description: Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d39dc856e2ef6f36e4188dc2694a7c23f4033183
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030461"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a>тип ресурса androidDeviceOwnerKioskModeManagedFolder

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|folderName|String|Отображение имени папки|
|folderIdentifier|Строка|Уникальный идентификатор для папки|
|элементы|[коллекция androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)|Элементы, которые необходимо добавить в управляемой папке. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Отношения
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



