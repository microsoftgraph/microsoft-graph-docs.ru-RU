---
title: Тип ресурса Апплеапплиститем
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2583c617ae34d60e83194f5136efcc6c51f06826
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021492"
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






