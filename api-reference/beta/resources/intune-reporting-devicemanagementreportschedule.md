---
title: Тип ресурса Девицеманажементрепортсчедуле
description: Сущность, представляющая расписание доставки отчетов
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea065d4f01472a907497cee612253e87b1ffd031
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079825"
---
# <a name="devicemanagementreportschedule-resource-type"></a>Тип ресурса Девицеманажементрепортсчедуле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая расписание доставки отчетов

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементрепортсчедулес](../api/intune-reporting-devicemanagementreportschedule-list.md)|Коллекция [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Список свойств и связей объектов [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Получение Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Чтение свойств и связей объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Создание Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Создание нового объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Удаление Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-delete.md)|Нет|Удаляет объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md).|
|[Обновление Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Обновление свойств объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|
|репортсчедуленаме|String|Имя расписания|
|subject|String|Тема запланированных отчетов, которые доставляются|
|письма|Коллекция String|Сообщения электронной почты, на которые доставляются запланированные отчеты|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Периодичность запланированной доставки отчета. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Время, когда начинается доставка запланированных отчетов|
|endDateTime|DateTimeOffset|Время окончания доставки запланированных отчетов|
|userId|String|Идентификатор пользователя, создавшего отчет|
|репортнаме|String|Имя отчета|
|filter|String|Фильтры, примененные к отчету|
|select|Коллекция String|Столбцы, выбранные из отчета|
|orderBy|Коллекция String|Упорядочение столбцов в отчете|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат запланированного отчета. Возможные значения: `csv`, `pdf`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```






