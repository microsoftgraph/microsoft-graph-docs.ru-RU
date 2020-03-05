---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67c1a4b4a9ac570b4acd71a1ce819f9705fd32e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528674"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>Тип ресурса Конфигуратионманажерклиентинформатион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Данные клиента Configuration Manager, синхронизированные из SCCM

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|клиентидентифиер|String|Идентификатор клиента Configuration Manager из SCCM|

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
  "clientIdentifier": "String"
}
```



