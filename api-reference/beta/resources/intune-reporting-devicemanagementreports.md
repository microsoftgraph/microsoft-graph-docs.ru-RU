---
title: тип ресурса deviceManagementReports
description: Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b91f2d8112c903b10f94268b3f885425b5b25a6c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869193"
---
# <a name="devicemanagementreports-resource-type"></a>тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Чтение свойств и связей [объекта deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)|
|[Обновление deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)|
|[действие getDeviceNonComplianceReport](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|Н/Д|
|[действие getPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|Н/Д|
|[действие getPolicyNonComplianceMetadata](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|Н/Д|
|[getPolicyNonComplianceSummaryReport action](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[getSettingNonComplianceReport action](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Stream|Н/Д|
|[действие getReportFilters](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Stream|Н/Д|
|[getHistoricalReport action](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Stream|Н/Д|
|[getConfigurationPolicyNonComplianceSummaryReport action](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[getConfigurationPolicyNonComplianceReport action](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancereport.md)|Stream|Н/Д|
|[getConfigurationSettingNonComplianceReport action](../api/intune-reporting-devicemanagementreports-getconfigurationsettingnoncompliancereport.md)|Stream|Н/Д|
|[getDeviceManagementIntentSettingsReport action](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentsettingsreport.md)|Stream|Н/Д|
|[getCompliancePolicyNonComplianceSummaryReport action](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[действие getCompliancePolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancereport.md)|Stream|Н/Д|
|[действие getComplianceSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancesettingnoncompliancereport.md)|Stream|Н/Д|
|[действие getCachedReport](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта|

## <a name="relationships"></a>Связи
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




