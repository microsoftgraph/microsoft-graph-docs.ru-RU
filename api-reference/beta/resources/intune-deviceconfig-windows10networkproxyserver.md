---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f02444a1cfccd2638f9fa6872b6b35dab649287
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786679"
---
# <a name="windows10networkproxyserver-resource-type"></a>Тип ресурса windows10NetworkProxyServer

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика прокси-сервера сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|address|String|Адрес прокси-сервера. Укажите адрес в формате <server>\[":"<port>\]|
|exceptions|Коллекция String|Адреса, которые не должны использовать прокси-сервер. Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.|
|useForLocalAddresses|Boolean|Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).|

## <a name="relationships"></a>Связи
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



