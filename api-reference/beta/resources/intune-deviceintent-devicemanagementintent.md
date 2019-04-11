---
title: Тип ресурса Девицеманажементинтент
description: Сущность, которая представляет цель применения параметров к устройству
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2de7d4e8c177317aa220d6aafbba4bda8b7fe299
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780926"
---
# <a name="devicemanagementintent-resource-type"></a>Тип ресурса Девицеманажементинтент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, которая представляет цель применения параметров к устройству

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентс](../api/intune-deviceintent-devicemanagementintent-list.md)|Коллекция [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md)|Список свойств и связей объектов [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Получение Девицеманажементинтент](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Чтение свойств и связей объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Создание Девицеманажементинтент](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Создание нового объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Удаление Девицеманажементинтент](../api/intune-deviceintent-devicemanagementintent-delete.md)|Нет|Удаляет объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md).|
|[Обновление Девицеманажементинтент](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Обновление свойств объекта [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Действие updateSettings](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|Нет|Н/Д|
|[Действие назначения](../api/intune-deviceintent-devicemanagementintent-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор намерения|
|displayName|String|Имя пользователя для данного отображаемого имени|
|description|String|Описание, заданное пользователем|
|isAssigned|Boolean|Указывает, назначена ли пользователю задача|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения намерения|
|templateId|String|Идентификатор шаблона, на основе которого была создана эта цель (при наличии)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|settings|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Набор всех параметров, которые необходимо применить|
|categories|Коллекция [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Коллекция настроек категорий|
|assignments|Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Коллекция назначений|
|deviceSettingStateSummaries|Коллекция [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Набор параметров и их состояний, а также количество устройств, которые относятся к соответствующему состоянию для всех параметров в цели|
|deviceStates|Коллекция [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Коллекция состояний всех устройств, к которым применяется цель|
|Усерстатес|Коллекция [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Коллекция состояний всех пользователей, к которым применяется цель|
|Девицестатесуммари|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Сводка состояний устройств и счетчиков устройств, которые относятся к соответствующему состоянию для всех устройств, к которым применяется цель|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Сводка по состояниям пользователей и количества пользователей, относящихся к соответствующему состоянию для всех пользователей, к которым применяется цель|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String"
}
```





