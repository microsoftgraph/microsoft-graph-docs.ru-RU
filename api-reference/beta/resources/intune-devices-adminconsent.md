---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f0f60f39c676fb8c6aca5144b2aa3b561b7cbaf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785177"
---
# <a name="adminconsent-resource-type"></a>Тип ресурса Adminconsent.

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



