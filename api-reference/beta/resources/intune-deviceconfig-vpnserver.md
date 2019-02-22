---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dd09e7ab0280120dd207424a862696ba087e20c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170464"
---
# <a name="vpnserver-resource-type"></a>Тип ресурса Vpnserver.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение VPN-сервера.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание.|
|address|String|Адрес (IP-адрес, полное ДОМЕНное имя или URL-адрес)|
|Исдефаултсервер|Логический|Сервер по умолчанию.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```




