---
title: тип ресурса deviceHealthScriptRunSchedule
description: Базовый тип расписания запуска скрипта для здоровья устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc910ae357bae0ac42f6e699de9c530a3da04a412ef36852098e97c937124d95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206342"
---
# <a name="devicehealthscriptrunschedule-resource-type"></a>тип ресурса deviceHealthScriptRunSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип расписания запуска скрипта для здоровья устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|X значение каждые х часов для почасового расписания, каждые х дней для ежедневного расписания, каждые х недель для еженедельного расписания, каждые х месяцев для ежемесячного расписания. Допустимые значения от 1 до 23|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": 1024
}
```




