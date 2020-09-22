---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09db43661113de84712a8228af047ca1683c383
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060904"
---
# <a name="adminconsent-resource-type"></a>Тип ресурса Adminconsent.

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о согласия администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|шареапнсдата|[админконсентстате](../resources/intune-devices-adminconsentstate.md)|Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple. Возможные значения: `notConfigured`, `granted`, `notGranted`.|
|шареусерекспериенцеаналитиксдата|[админконсентстате](../resources/intune-devices-adminconsentstate.md)|Получает или задает согласие администратора для совместного использования данных аналитики взаимодействия с пользователем. Возможные значения: `notConfigured`, `granted`, `notGranted`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```






