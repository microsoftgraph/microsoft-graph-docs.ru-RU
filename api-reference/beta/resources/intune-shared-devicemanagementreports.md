---
title: тип ресурса deviceManagementReports
description: Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c88430dc050c913d16886395f0f6481a579d75a5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127048"
---
# <a name="devicemanagementreports-resource-type"></a>тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-shared-devicemanagementreports.md)|Чтение свойств и связей [объекта deviceManagementReports.](../resources/intune-shared-devicemanagementreports.md)|
|[Обновление deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-shared-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports.](../resources/intune-shared-devicemanagementreports.md)|
|[действие getDeviceNonComplianceReport](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|Н/Д|
|[действие getPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|Н/Д|
|[действие getPolicyNonComplianceMetadata](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|Н/Д|
|[getPolicyNonComplianceSummaryReport action](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[getSettingNonComplianceReport action](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Stream|Н/Д|
|[действие getReportFilters](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Stream|Н/Д|
|[getHistoricalReport action](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Stream|Н/Д|
|[действие getCachedReport](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|cachedReportConfigurations|[коллекция deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Объект, представляющий конфигурацию кэшного отчета|
|exportJobs|[коллекция deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Объект, представляющий задание по экспорту отчета|
|reportSchedules|[коллекция deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Объект, представляющий расписание доставки отчетов|

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





