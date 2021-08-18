---
title: Тип ресурса windowsDeviceAzureADAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01b4e0e9f1b1e513f499969607a5d1befbc01709d38bf1e8ec475a4adaf36b25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249848"
---
# <a name="windowsdeviceazureadaccount-resource-type"></a>Тип ресурса windowsDeviceAzureADAccount

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д


Наследуется от ресурса [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|password|Строка|Н/Д Наследуется от ресурса [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|
|userPrincipalName|String|Н/Д|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceAzureADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceAzureADAccount",
  "password": "String",
  "userPrincipalName": "String"
}
```




