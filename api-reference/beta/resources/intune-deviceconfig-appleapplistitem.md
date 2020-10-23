---
title: Тип ресурса Апплеапплиститем
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 831991580d2b3d667011d84179a73957c6eeb200
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703925"
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





