---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42a92fd725c9f0b99037825c240dd017bf6c9c82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060778"
---
# <a name="comanageddevicessummary-resource-type"></a>Тип ресурса Команажеддевицессуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводные данные для совместно управляемых устройств

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|инвенторикаунт|Int32|Количество устройств с свунгом инвентаризации. Это свойство доступно только для чтения.|
|комплианцеполицикаунт|Int32|Количество устройств с Комплианцеполици свунг. Это свойство доступно только для чтения.|
|ресаурцеакцесскаунт|Int32|Количество устройств с Ресаурцеакцесс свунг. Это свойство доступно только для чтения.|
|конфигуратионсеттингскаунт|Int32|Количество устройств с Конфигуратионсеттингс свунг. Это свойство доступно только для чтения.|
|виндовсупдатефорбусинесскаунт|Int32|Количество устройств с Виндовсупдатефорбусинесс свунг. Это свойство доступно только для чтения.|
|ендпоинтпротектионкаунт|Int32|Количество устройств с Ендпоинтпротектион свунг. Это свойство доступно только для чтения.|
|модернаппскаунт|Int32|Количество устройств с Модернаппс свунг. Это свойство доступно только для чтения.|
|оффицеаппскаунт|Int32|Количество устройств с Оффицеаппс свунг. Это свойство доступно только для чтения.|
|тоталкоманажедкаунт|Int32|Количество совместно управляемых устройств. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```






