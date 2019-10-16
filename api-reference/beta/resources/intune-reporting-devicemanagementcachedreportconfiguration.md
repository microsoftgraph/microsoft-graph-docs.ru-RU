---
title: Тип ресурса Девицеманажементкачедрепортконфигуратион
description: Сущность, представляющая конфигурацию кэшированного отчета
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8bd2b3ef44c5522011f15f2a1335b325a666f63c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539045"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a>Тип ресурса Девицеманажементкачедрепортконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая конфигурацию кэшированного отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементкачедрепортконфигуратионс](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|Коллекция [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Список свойств и связей объектов [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .|
|[Получение Девицеманажементкачедрепортконфигуратион](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Чтение свойств и связей объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .|
|[Создание Девицеманажементкачедрепортконфигуратион](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .|
|[Удаление Девицеманажементкачедрепортконфигуратион](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|Нет|Удаляет объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).|
|[Обновление Девицеманажементкачедрепортконфигуратион](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Обновление свойств объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этой сущности|
|репортнаме|String|Имя отчета|
|filter|String|Фильтры, применяемые при создании отчета.|
|select|Коллекция String|Столбцы, выбранные из отчета|
|orderBy|Коллекция String|Упорядочение столбцов в отчете|
|status|[девицеманажементрепортстатус](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние кэшированного отчета. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|ластрефрешдатетиме|DateTimeOffset|Время последнего обновления кэшированного отчета|
|expirationDateTime|DateTimeOffset|Время истечения срока действия кэшированного отчета|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



