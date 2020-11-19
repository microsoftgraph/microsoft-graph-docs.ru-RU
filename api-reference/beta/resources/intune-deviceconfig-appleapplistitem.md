---
title: Тип ресурса Апплеапплиститем
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a95905ef8076883ebdeea4a5ea6973017e511fee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283751"
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
|name|String|Имя приложения, унаследованное от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|publisher|String|Издатель приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|URL-адрес хранилища приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|
|appId|String|Идентификатор приложения или пакета приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)|

## <a name="relationships"></a>Связи
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




