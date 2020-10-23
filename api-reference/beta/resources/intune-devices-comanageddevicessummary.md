---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1e0266151c2b32baa0c5d66ea1341eee6da28b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725507"
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
|тоталкоманажедкаунт|Int32|Количество устройств Co-Managed. Это свойство доступно только для чтения.|

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





