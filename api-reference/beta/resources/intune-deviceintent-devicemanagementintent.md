---
title: тип ресурса deviceManagementIntent
description: Сущность, которая представляет намерение применить параметры к устройству
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 465abb5a003817f596eb70067b8ac6b5a28e94e7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58759437"
---
# <a name="devicemanagementintent-resource-type"></a>тип ресурса deviceManagementIntent

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, которая представляет намерение применить параметры к устройству

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntents](../api/intune-deviceintent-devicemanagementintent-list.md)|[коллекция deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Список свойств и связей [объектов deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Get deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Чтение свойств и связей [объекта deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Создание deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Создание нового [объекта deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Удаление deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-delete.md)|Нет|Удаляет [устройствоManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).|
|[Обновление deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Обновление свойств объекта [deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Действие updateSettings](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|Нет|Н/Д|
|[действие migrateToTemplate](../api/intune-deviceintent-devicemanagementintent-migratetotemplate.md)|Нет|Н/Д|
|[действие createCopy](../api/intune-deviceintent-devicemanagementintent-createcopy.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Н/Д|
|[Действие assign](../api/intune-deviceintent-devicemanagementintent-assign.md)|Нет|Н/Д|
|[сравнение функции](../api/intune-deviceintent-devicemanagementintent-compare.md)|[коллекция deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID намерения|
|displayName|Строка|Имя отображения, заданное пользователю|
|description|Строка|Описание пользователя|
|isAssigned|Boolean|Означает, назначены ли намерения пользователям|
|lastModifiedDateTime|DateTimeOffset|Когда намерение было изменено в последний раз|
|templateId|String|ID шаблона, который был создан из (если таково)|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров, которые необходимо применить|
|categories|[коллекция deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Коллекция категорий параметров в пределах намерения|
|assignments|[коллекция deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Коллекция назначений|
|deviceSettingStateSummaries|[коллекция deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Коллекция параметров и их состояния и количество устройств, которые относятся к соответствующему штату для всех параметров в пределах намерения|
|deviceStates|[коллекция deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Коллекция состояния всех устройств, на которые применяется намерение|
|userStates|[коллекция deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Коллекция состояния всех пользователей, к которые применяется намерение|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Сводка состояния устройств и количество устройств, которые относятся к соответствующему состоянии для всех устройств, на которые применяется намерение|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Сводка о состояниях пользователей и подсчетах пользователей, принадлежащих к соответствующему государству для всех пользователей, к которые применяется намерение|

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



