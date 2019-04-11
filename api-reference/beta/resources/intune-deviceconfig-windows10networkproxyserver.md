---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 120eff89a01434803c1e2f4f5ba84d3f088e1022
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796362"
---
# <a name="windows10networkproxyserver-resource-type"></a>Тип ресурса windows10NetworkProxyServer

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика прокси-сервера сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|address|String|Адрес прокси-сервера. Укажите адрес в формате <server>\[":"<port>\]|
|exceptions|Коллекция String|Адреса, которые не должны использовать прокси-сервер. Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.|
|useForLocalAddresses|Boolean|Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```





