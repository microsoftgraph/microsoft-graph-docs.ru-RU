---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd4a62fdc60378260b1eceda22cc5020a16cbd9d4a810218552bb32ab988c739
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223468"
---
# <a name="androidmobileappidentifier-resource-type"></a>Тип ресурса androidMobileAppIdentifier

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Идентификатор приложения для Android.


Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|packageId|String|Идентификатор приложения, указанный в магазине Google Play.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




