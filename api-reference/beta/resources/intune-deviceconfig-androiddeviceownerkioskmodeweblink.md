---
title: тип ресурса androidDeviceOwnerKioskModeWeblink
description: Веб-ссылки на управляемом домашнем экране владельца android-устройств
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: edaa003fc6f963e43bf55ed8f0833cd59ca2a56e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101809"
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
|link|String|Ссылка для веб-ссылки|

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



