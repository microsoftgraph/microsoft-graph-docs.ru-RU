---
title: Тип ресурса androidDeviceOwnerKioskModeManagedFolderReference
description: Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f454abc8edb54e1ee2ed2e9a6984e8e9e39e29d2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162558"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a>Тип ресурса androidDeviceOwnerKioskModeManagedFolderReference

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране


Наследуется [от androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|folderName|String|Имя папки|
|folderIdentifier|String|Уникальный идентификатор папки|

## <a name="relationships"></a>Связи
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




