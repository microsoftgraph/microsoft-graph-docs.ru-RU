---
title: Тип ресурса Девицеманажементекспортжоб
description: Сущность, представляющая задание для экспорта отчета
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1ee8c07f6083d7e6f5b5b061bd87b3438683912
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538541"
---
# <a name="devicemanagementexportjob-resource-type"></a>Тип ресурса Девицеманажементекспортжоб

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая задание для экспорта отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементекспортжобс](../api/intune-reporting-devicemanagementexportjob-list.md)|Коллекция [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Список свойств и связей объектов [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Получение Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-get.md)|[девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Чтение свойств и связей объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Создание Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-create.md)|[девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Создание нового объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Удаление Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-delete.md)|Нет|Удаляет объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Обновление Девицеманажементекспортжоб](../api/intune-reporting-devicemanagementexportjob-update.md)|[девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md)|Обновление свойств объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|
|репортнаме|String|Имя отчета|
|filter|String|Фильтры, примененные к отчету|
|select|Коллекция String|Столбцы, выбранные из отчета|
|orderBy|Коллекция String|Упорядочение столбцов в отчете|
|format|[девицеманажементрепортфилеформат](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат экспортированного отчета. Возможные значения: `csv`, `pdf`.|
|снапшотид|String|Моментальный снимок является идентифицируемым подмножеством набора данных, представленным Репортнаме. Здесь можно использовать идентификатор sessionId или Качедрепортконфигуратион. Если указан идентификатор sessionId, фильтрация, выбор и OrderBy применяются к данным, представленным в sessionId. Filter, SELECT и OrderBy не могут указываться вместе с идентификатором Качедрепортконфигуратион.|
|status|[девицеманажементрепортстатус](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние задания экспорта. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
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
  "orderBy": [
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



