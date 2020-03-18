---
title: Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари
description: Объект Entity, представляющий сводку состояний параметров устройства для намерения
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a351f3ca7dd778592150605ca7a491212f4e51d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785430"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Entity, представляющий сводку состояний параметров устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентдевицесеттингстатесуммариес](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|Коллекция [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Список свойств и связей объектов [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Получение Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Создание Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Создание нового объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Удаление Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|Нет|Удаляет объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).|
|[Обновление Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
|settingName|String|Имя параметра|
|комплианткаунт|Int32|Количество устройств, соответствующих требованиям.|
|conflictCount|Int32|Количество конфликтующих устройств|
|errorCount|Int32|Количество устройств с ошибками.|
|нонкомплианткаунт|Int32|Количество устройств, не соответствующих требованиям|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|ремедиатедкаунт|Int32|Количество исправленных устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": 1024,
  "conflictCount": 1024,
  "errorCount": 1024,
  "nonCompliantCount": 1024,
  "notApplicableCount": 1024,
  "remediatedCount": 1024
}
```



