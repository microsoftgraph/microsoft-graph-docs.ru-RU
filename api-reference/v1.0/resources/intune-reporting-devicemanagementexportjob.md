---
title: Тип ресурса deviceManagementExportJob
description: Сущность, представляющая задание для экспорта отчета
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de9cf79f34b3f1d6c69ff3fb3d4018995b01c577
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730310"
---
# <a name="devicemanagementexportjob-resource-type"></a>Тип ресурса deviceManagementExportJob

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая задание для экспорта отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[Коллекция deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Список свойств и связей объектов [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Получение объекта deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Чтение свойств и связей объекта [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Создание объекта deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Создайте объект [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Удаление объекта deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|Нет|Удаляет [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Обновление объекта deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Обновление свойств объекта [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|
|reportName|String|Имя отчета|
|filter|String|Фильтры, примененные к отчету|
|select|Коллекция String|Столбцы, выбранные в отчете|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат экспортированного отчета. Возможные значения: `csv`, `pdf`.|
|snapshotId|String|Моментальный снимок — это идентифицируемое подмножество набора данных, представленного reportName. Здесь можно использовать идентификатор sessionId или CachedReportConfiguration. Если указан идентификатор сеанса, фильтр, select и OrderBy применяются к данным, представленным sessionId. Параметры Filter, Select и OrderBy нельзя указать вместе с идентификатором CachedReportConfiguration.|
|localizationType|[DeviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Настраивает способ локализации запрашиваемого задания экспорта. Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние задания экспорта. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Временное расположение экспортированного отчета|
|requestDateTime|DateTimeOffset|Время запроса экспортированного отчета|
|expirationDateTime|DateTimeOffset|Время истечения срока действия экспортированного отчета|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExportJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "format": "String",
  "snapshotId": "String",
  "localizationType": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```





