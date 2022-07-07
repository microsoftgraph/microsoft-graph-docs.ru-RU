---
title: Тип ресурса deviceManagementReports
description: Одноэлементная сущность, которая выступает в качестве контейнера для всех функций отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b1394eb01dfa8f60be7071ea381bc6eb584eb7b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671320"
---
# <a name="devicemanagementreports-resource-type"></a>Тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементная сущность, которая выступает в качестве контейнера для всех функций отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Чтение свойств и связей объекта [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .|
|[Обновление deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .|
|[Действие getDeviceNonComplianceReport](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|Н/Д|
|[Действие getNoncompliantDevicesAndSettingsReport](../api/intune-reporting-devicemanagementreports-getnoncompliantdevicesandsettingsreport.md)|Stream|Н/Д|
|[Действие getPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|Н/Д|
|[Действие getPolicyNonComplianceMetadata](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|Н/Д|
|[Действие getPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[Действие getSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Stream|Н/Д|
|[Действие getReportFilters](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Stream|Н/Д|
|[Действие getHistoricalReport](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Stream|Н/Д|
|[Действие getConfigurationPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[Действие getConfigurationPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancereport.md)|Stream|Н/Д|
|[Действие getConfigurationSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationsettingnoncompliancereport.md)|Stream|Н/Д|
|[Действие getDeviceManagementIntentSettingsReport](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentsettingsreport.md)|Stream|Н/Д|
|[Действие getDeviceManagementIntentPerSettingContributingProfiles](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentpersettingcontributingprofiles.md)|Stream|Н/Д|
|[Действие getCompliancePolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancesummaryreport.md)|Stream|Н/Д|
|[Действие getCompliancePolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancereport.md)|Stream|Н/Д|
|[Действие getComplianceSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancesettingnoncompliancereport.md)|Stream|Н/Д|
|[Действие getCachedReport](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|cachedReportConfigurations|[Коллекция deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Сущность, представляющая конфигурацию кэшированного отчета|
|exportJobs|[Коллекция deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Сущность, представляющая задание для экспорта отчета|

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




