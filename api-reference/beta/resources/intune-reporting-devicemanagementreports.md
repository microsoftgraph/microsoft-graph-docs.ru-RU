---
title: Тип ресурса Девицеманажементрепортс
description: Одноэлементный объект, служащий контейнером для всех функций отчетов.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8fa5979339f471fbe6d0fc5aa046ee8cdd00c19b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539213"
---
# <a name="devicemanagementreports-resource-type"></a>Тип ресурса Девицеманажементрепортс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-get.md)|[девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md)|Чтение свойств и связей объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .|
|[Обновление Девицеманажементрепортс](../api/intune-reporting-devicemanagementreports-update.md)|[девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md)|Обновление свойств объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .|
|[действие Жетдевиценонкомплианцерепортс](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereports.md)|Stream|Н/Д|
|[действие Жетполицинонкомплианцерепортс](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereports.md)|Stream|Н/Д|
|[действие Жетдевиценонкомплианцерепорт](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|Н/Д|
|[действие Жетполицинонкомплианцерепорт](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|Н/Д|
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



