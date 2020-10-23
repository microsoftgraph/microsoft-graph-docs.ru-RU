---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b99db60922a93353cd1cc2cb6b85ff6b1241efe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690240"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>Тип ресурса Конфигуратионманажерклиентинформатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Данные клиента Configuration Manager, синхронизированные из SCCM

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|клиентидентифиер|Строка|Идентификатор клиента Configuration Manager из SCCM|
|Блокировка|Логический|Состояние блокировки клиента Configuration Manager из SCCM|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```





