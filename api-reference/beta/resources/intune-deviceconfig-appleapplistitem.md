---
title: тип ресурса appleAppListItem
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8e88bae9f25bc2268d1dca43c7d33dcb1c928f638a9b59135e3ec5dcdb61373
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213209"
---
# <a name="appleapplistitem-resource-type"></a>тип ресурса appleAppListItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет приложение в списке управляемых приложений Apple


Наследует [от appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя приложения, унаследованные от [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|publisher|String|Издатель приложения, унаследованный от [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|URL-адрес магазина приложения, унаследованный от [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appId|String|Идентификатор приложения или пакета приложения, унаследованный от [appListItem](../resources/intune-deviceconfig-applistitem.md)|

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




