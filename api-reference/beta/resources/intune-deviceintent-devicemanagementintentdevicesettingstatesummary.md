---
title: Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари
description: Объект Entity, представляющий сводку состояний параметров устройства для намерения
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c3e6a3630d3e28e62555db25565ab916dc7a91
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524059"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентдевицесеттингстатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Entity, представляющий сводку состояний параметров устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентдевицесеттингстатесуммариес](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|Коллекция [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Список свойств и связей объектов [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Получение Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[Девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Создание Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[Девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Создание нового объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Удаление Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|Нет|Удаляет объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).|
|[Обновление Девицеманажементинтентдевицесеттингстатесуммари](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[Девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
|settingName|String|Имя параметра|
|Комплианткаунт|Int32|Количество устройств, соответствующих требованиям.|
|conflictCount|Int32|Количество конфликтующих устройств|
|errorCount|Int32|Количество устройств с ошибками.|
|Нонкомплианткаунт|Int32|Количество устройств, не соответствующих требованиям|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|Ремедиатедкаунт|Int32|Количество исправленных устройств.|

## <a name="relationships"></a>Отношения
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







