---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f592ba7900f0761a24b02495dc337046b615bb1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793467"
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
  "officeAppsCount": 1024
}
```



