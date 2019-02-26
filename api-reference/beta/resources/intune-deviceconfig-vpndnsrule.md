---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545c0dd8a84f19888452261e350a9b347061595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158508"
---
# <a name="vpndnsrule-resource-type"></a>Тип ресурса Впнднсруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила DNS для VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Расширением.|
|серверы|Коллекция строк|Серверами.|
|Проксисерверури|String|URI прокси-сервера.|
|автоТриггер|Логический|Автоматически подключаться к ВИРТУАЛЬНОЙ частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.|
|persistent|Логический|Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```




