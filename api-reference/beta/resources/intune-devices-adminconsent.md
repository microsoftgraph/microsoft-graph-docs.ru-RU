---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d45249024e7d3766bfedb716c151a495a92daa75
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462462"
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

## <a name="relationships"></a>Отношения
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



