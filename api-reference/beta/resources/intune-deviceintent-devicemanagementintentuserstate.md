---
title: тип ресурса deviceManagementIntentUserState
description: Сущность, представляюая состояние пользователя для намерения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5b0c16a99a66acb502bdc65b3ccfc7f0e4a984d328e1b46ec30982ef714a271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252930"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>тип ресурса deviceManagementIntentUserState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая состояние пользователя для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentUserStates](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[коллекция deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Список свойств и связей [объектов deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Get deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Чтение свойств и связей [объекта deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Создание deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Создание нового [объекта deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Удаление deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|Нет|Удаляет [устройствоManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).|
|[Обновление deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Обновление свойств объекта [deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|The ID|
|userPrincipalName|String|Основное имя пользователя, которое сообщается на устройстве|
|userName|String|Имя пользователя, которое сообщается на устройстве|
|deviceCount|Int32|Количество устройств, принадлежащих пользователю для намерения|
|lastReportedDateTime|DateTimeOffset|Последнее измененное время даты отчета о намерениях|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Состояние пользователя для намерения. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```




