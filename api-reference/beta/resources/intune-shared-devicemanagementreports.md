---
title: Тип ресурса Девицеманажементрепортс
description: Одноэлементный объект, служащий контейнером для всех функций отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61ad0d59ef17cc09b65513914a4e87e390f41f0a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337105"
---
# <a name="devicemanagementreports-resource-type"></a>Тип ресурса Девицеманажементрепортс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-shared-devicemanagementreports.md)|Чтение свойств и связей объекта [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md) .|
|[Обновление Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-shared-devicemanagementreports.md)|Обновление свойств объекта [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md) .|
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

## <a name="relationships"></a>Связи
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




