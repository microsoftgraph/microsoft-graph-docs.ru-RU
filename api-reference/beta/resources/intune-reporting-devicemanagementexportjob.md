---
title: Тип ресурса Девицеманажементекспортжоб
description: Сущность, представляющая задание для экспорта отчета
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e44057e786126003802cada7320329167a3c97fe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772554"
---
# <a name="devicemanagementexportjob-resource-type"></a>Тип ресурса Девицеманажементекспортжоб

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая задание для экспорта отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементекспортжобс](../api/intune-reporting-devicemanagementexportjob-list.md)|Коллекция [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Список свойств и связей объектов [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Получение Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Чтение свойств и связей объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Создание Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Создание нового объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Удаление Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-delete.md)|Нет|Удаляет объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Обновление Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Обновление свойств объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|
|репортнаме|String|Имя отчета|
|filter|String|Фильтры, примененные к отчету|
|select|Коллекция String|Столбцы, выбранные из отчета|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат экспортированного отчета. Возможные значения: `csv`, `pdf`.|
|снапшотид|String|Моментальный снимок является идентифицируемым подмножеством набора данных, представленным Репортнаме. Здесь можно использовать идентификатор sessionId или Качедрепортконфигуратион. Если указан идентификатор sessionId, фильтрация, выбор и OrderBy применяются к данным, представленным в sessionId. Filter, SELECT и OrderBy не могут указываться вместе с идентификатором Качедрепортконфигуратион.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние задания экспорта. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Временное расположение экспортируемого отчета|
|рекуестдатетиме|DateTimeOffset|Время запроса экспорта отчета|
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
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



