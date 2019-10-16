---
title: Тип ресурса Девицеманажементрепортсчедуле
description: Сущность, представляющая расписание доставки отчетов
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 231f1f84acd294c340984c0c375bb87ceba94f95
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538849"
---
# <a name="devicemanagementreportschedule-resource-type"></a>Тип ресурса Девицеманажементрепортсчедуле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая расписание доставки отчетов

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементрепортсчедулес](../api/intune-reporting-devicemanagementreportschedule-list.md)|Коллекция [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Список свойств и связей объектов [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Получение Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-get.md)|[девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Чтение свойств и связей объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Создание Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-create.md)|[девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Создание нового объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Удаление Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-delete.md)|Нет|Удаляет объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md).|
|[Обновление Девицеманажементрепортсчедуле](../api/intune-reporting-devicemanagementreportschedule-update.md)|[девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md)|Обновление свойств объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этой сущности|
|репортсчедуленаме|String|Имя расписания|
|subject|String|Тема запланированных отчетов, которые доставляются|
|письма|Коллекция String|Сообщения электронной почты, на которые доставляются запланированные отчеты|
|recurrence|[девицеманажементсчедуледрепортрекурренце](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Периодичность запланированной доставки отчета. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Время, когда начинается доставка запланированных отчетов|
|endDateTime|DateTimeOffset|Время окончания доставки запланированных отчетов|
|userId|String|Идентификатор пользователя, создавшего отчет|
|репортнаме|String|Имя отчета|
|filter|String|Фильтры, примененные к отчету|
|select|Коллекция String|Столбцы, выбранные из отчета|
|orderBy|Коллекция String|Упорядочение столбцов в отчете|
|format|[девицеманажементрепортфилеформат](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат запланированного отчета. Возможные значения: `csv`, `pdf`.|

## <a name="relationships"></a>Связи
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



