---
title: Тип ресурса Девицеманажементинтентусерстатесуммари
description: Сущность, представляющая сводную информацию о состоянии пользователя для намерения
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc53020966717c2f9324e9fddef9b7f0173b0eb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528824"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентусерстатесуммари

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая сводную информацию о состоянии пользователя для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементинтентусерстатесуммари](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|
|[Обновление Девицеманажементинтентусерстатесуммари](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
|conflictCount|Int32|Количество пользователей в конфликте|
|errorCount|Int32|Количество пользователей с ошибками|
|failedCount|Int32|Количество пользователей с ошибками|
|notApplicableCount|Int32|Количество неприменимых пользователей|
|successCount|Int32|Количество успешных пользователей|

## <a name="relationships"></a>Связи
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



