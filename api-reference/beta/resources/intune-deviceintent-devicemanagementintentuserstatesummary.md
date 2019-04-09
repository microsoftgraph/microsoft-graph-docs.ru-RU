---
title: Тип ресурса Девицеманажементинтентусерстатесуммари
description: Сущность, представляющая сводную информацию о состоянии пользователя для намерения
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c930b19e604aaf3867260e359a2b7fcb12153762
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523996"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентусерстатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая сводную информацию о состоянии пользователя для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементинтентусерстатесуммари](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[Девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|
|[Обновление Девицеманажементинтентусерстатесуммари](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[Девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
|conflictCount|Int32|Количество пользователей в конфликте|
|errorCount|Int32|Количество пользователей с ошибками|
|failedCount|Int32|Количество пользователей с ошибками|
|notApplicableCount|Int32|Количество неприменимых пользователей|
|successCount|Int32|Количество успешных пользователей|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```







