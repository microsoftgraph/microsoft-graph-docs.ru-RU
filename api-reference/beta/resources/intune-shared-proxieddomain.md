---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5edabc31761a3abd79a94bb700392923d2d54513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151207"
---
# <a name="proxieddomain-resource-type"></a>Тип ресурса proxiedDomain

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Проксируемый домен

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddressOrFQDN|Строка|IP-адрес или полное доменное имя|
|proxy|Строка|IP-адрес или полное ДОМЕНное имя прокси|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```




