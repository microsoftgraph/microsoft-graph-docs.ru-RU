---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c46d3b44c28c7f07b5d0478acc3f82547b3819ee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466862"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>Тип ресурса Виндовскиоскактиведиректориграуп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения группы каталогов Azure для конфигурации киоска


Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupName|String|Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```



