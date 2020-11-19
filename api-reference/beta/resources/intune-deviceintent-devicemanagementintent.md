---
title: Тип ресурса Девицеманажементинтент
description: Сущность, которая представляет цель применения параметров к устройству
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d154418b0b888c4ef084cb7039a493ac0441ec7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275890"
---
# <a name="devicemanagementintent-resource-type"></a>Тип ресурса Девицеманажементинтент

Пространство имен: microsoft.graph

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
|[действие Креатекопи](../api/intune-deviceintent-devicemanagementintent-createcopy.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Н/Д|
|[Действие assign](../api/intune-deviceintent-devicemanagementintent-assign.md)|Нет|Н/Д|
|[Функция Compare](../api/intune-deviceintent-devicemanagementintent-compare.md)|Коллекция [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор намерения|
|displayName|String|Имя пользователя для данного отображаемого имени|
|description|String|Описание, заданное пользователем|
|isAssigned|Boolean|Указывает, назначена ли пользователю задача|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения намерения|
|templateId|String|Идентификатор шаблона, на основе которого была создана эта цель (при наличии)|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|

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




