---
title: Тип ресурса Девицеманажементрепортс
description: Одноэлементный объект, служащий контейнером для всех функций отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d64f5ce049c73b74f105f3899ccf218e3c82fc85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039379"
---
# <a name="devicemanagementreports-resource-type"></a>Тип ресурса Девицеманажементрепортс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Чтение свойств и связей объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .|
|[Обновление Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Обновление свойств объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .|
|[действие Жетдевиценонкомплианцерепорт](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|Н/Д|
|[действие Жетполицинонкомплианцерепорт](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|Н/Д|
|[действие Жетполицинонкомплианцеметадата](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|Н/Д|
|[действие Жетполицинонкомплианцесуммарирепорт](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[действие Жетсеттингнонкомплианцерепорт](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Stream|Н/Д|
|[действие Жетрепортфилтерс](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Stream|Н/Д|
|[действие Жесисторикалрепорт](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Stream|Н/Д|
|[действие Жеткачедрепорт](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|качедрепортконфигуратионс|Коллекция [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Сущность, представляющая конфигурацию кэшированного отчета|
|експортжобс|Коллекция [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Сущность, представляющая задание для экспорта отчета|
|репортсчедулес|Коллекция [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Сущность, представляющая расписание доставки отчетов|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```






