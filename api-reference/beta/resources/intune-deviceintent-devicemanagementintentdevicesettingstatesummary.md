---
title: Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари
description: Объект Entity, представляющий сводку состояний параметров устройства для намерения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31a4f50115125d4e3f2a5c965d0d80e27fbfdf49
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691444"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари

Пространство имен: microsoft.graph

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
|id|Строка|Идентификатор|
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





