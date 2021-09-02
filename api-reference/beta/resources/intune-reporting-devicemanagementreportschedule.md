---
title: тип ресурса deviceManagementReportSchedule
description: Объект, представляющий расписание доставки отчетов
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ed97e1cebfec55a6ec9420ab818f208873daa2a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800347"
---
# <a name="devicemanagementreportschedule-resource-type"></a>тип ресурса deviceManagementReportSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий расписание доставки отчетов

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementReportSchedules](../api/intune-reporting-devicemanagementreportschedule-list.md)|[коллекция deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Список свойств и связей [объектов deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Get deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Чтение свойств и связей [объекта deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Создание deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Создание нового [объекта deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Удаление deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-delete.md)|Нет|Удаляет [устройствоManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Обновление deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Обновление свойств объекта [deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта|
|reportScheduleName|Строка|Имя расписания|
|subject|String|Тема запланированных отчетов, которые будут доставлены|
|электронные письма|Коллекция String|Сообщения электронной почты, на которые доставляются запланированные отчеты|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Частота доставки отчетов по расписанию. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Время начала доставки запланированных отчетов|
|endDateTime|DateTimeOffset|Время окончания доставки запланированных отчетов|
|userId|String|Id пользователя, создавшего отчет|
|reportName|Строка|Имя отчета|
|filter|Строка|Фильтры, применяемые в отчете|
|select|Коллекция String|Столбцы, выбранные из отчета|
|orderBy|Коллекция String|Порядок столбцов в отчете|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат запланированного отчета. Возможные значения: `csv`, `pdf`.|

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



