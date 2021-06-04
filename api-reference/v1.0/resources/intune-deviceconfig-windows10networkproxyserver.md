---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c561787c74649c6628768de691510524165f43f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742736"
---
# <a name="windows10networkproxyserver-resource-type"></a>Тип ресурса windows10NetworkProxyServer

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




