---
title: Тип ресурса Девицеманажементинтент
description: Сущность, которая представляет цель применения параметров к устройству
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ab1b6cd07bfa922f82cbd11e4f03aa2ba0a3515
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785437"
---
# <a name="devicemanagementintent-resource-type"></a>Тип ресурса Девицеманажементинтент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|[действие Мигратетотемплате](../api/intune-deviceintent-devicemanagementintent-migratetotemplate.md)|Нет|Н/Д|
|[Действие assign](../api/intune-deviceintent-devicemanagementintent-assign.md)|Нет|Н/Д|
|[Функция Compare](../api/intune-deviceintent-devicemanagementintent-compare.md)|Коллекция [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор намерения|
|displayName|Строка|Имя пользователя для данного отображаемого имени|
|description|String|Описание, заданное пользователем|
|isAssigned|Boolean|Указывает, назначена ли пользователю задача|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения намерения|
|templateId|String|Идентификатор шаблона, на основе которого была создана эта цель (при наличии)|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|параметры|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Набор всех параметров, которые необходимо применить|
|categories|Коллекция [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Коллекция настроек категорий|
|assignments|Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Коллекция назначений|
|deviceSettingStateSummaries|Коллекция [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Набор параметров и их состояний, а также количество устройств, которые относятся к соответствующему состоянию для всех параметров в цели|
|deviceStates|Коллекция [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Коллекция состояний всех устройств, к которым применяется цель|
|userStates|Коллекция [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Коллекция состояний всех пользователей, к которым применяется цель|
|девицестатесуммари|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Сводка состояний устройств и счетчиков устройств, которые относятся к соответствующему состоянию для всех устройств, к которым применяется цель|
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
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



