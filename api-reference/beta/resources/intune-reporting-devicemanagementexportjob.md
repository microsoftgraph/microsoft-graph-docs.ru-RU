---
title: тип ресурса deviceManagementExportJob
description: Объект, представляющий задание по экспорту отчета
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29f56794b23a508e3ffecdf6d380ac918b469625
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784774"
---
# <a name="devicemanagementexportjob-resource-type"></a>тип ресурса deviceManagementExportJob

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий задание по экспорту отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[коллекция deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Список свойств и связей объектов [deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Get deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Чтение свойств и связей [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Создание deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Создание нового [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Удаление deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|Нет|Удаляет [устройствоManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Обновление deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Обновление свойств объекта [deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта|
|reportName|Строка|Имя отчета|
|filter|Строка|Фильтры, применяемые в отчете|
|select|Коллекция String|Столбцы, выбранные из отчета|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат экспортируемого отчета. Возможные значения: `csv`, `pdf`.|
|snapshotId|Строка|Снимок — это идентифицируемый подмножество наборов данных, представленных в ReportName. Здесь можно использовать id sessionId или CachedReportConfiguration. Если задана sessionId, фильтр, выберите и OrderBy применяются к данным, представленным sessionId. Фильтр, выбор и OrderBy нельзя указать вместе с id CachedReportConfiguration.|
|ЛокализацияТип|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Настройка локализации запрашиваемого задания экспорта. Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние задания экспорта. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Временное расположение экспортируемого отчета|
|requestDateTime|DateTimeOffset|Время запроса экспортируемой отчетности|
|expirationDateTime|DateTimeOffset|Время истечения срока действия экспортируемой отчетности|

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



