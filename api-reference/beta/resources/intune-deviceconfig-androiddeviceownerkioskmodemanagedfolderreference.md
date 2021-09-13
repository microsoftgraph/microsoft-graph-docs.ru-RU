---
title: тип ресурса androidDeviceOwnerKioskModeManagedFolderReference
description: Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97276755676fbde8e41d4c5bac3fb1e381b7376d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030454"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a>тип ресурса androidDeviceOwnerKioskModeManagedFolderReference

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране


Наследует [от androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|folderName|String|Имя папки|
|folderIdentifier|Строка|Уникальный идентификатор для папки|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```



