---
title: Тип ресурса Апплеапплиститем
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470127"
---
# <a name="appleapplistitem-resource-type"></a>Тип ресурса Апплеапплиститем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет приложение в списке управляемых приложений Apple


Наследуется от [апплиститем](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|Строка|Имя приложения, унаследованное от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|publisher|String|Издатель приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|URL-адрес хранилища приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|appId|String|Идентификатор пакета приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



