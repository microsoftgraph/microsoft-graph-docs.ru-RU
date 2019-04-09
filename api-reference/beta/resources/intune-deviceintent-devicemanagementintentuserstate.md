---
title: Тип ресурса Девицеманажементинтентусерстате
description: Объект, представляющий состояние пользователя для намерения
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67d8a11816132d0867987c80325f100d5e9a1ecd
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524332"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>Тип ресурса Девицеманажементинтентусерстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий состояние пользователя для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентусерстатес](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|Коллекция [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Список свойств и связей объектов [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Получение Девицеманажементинтентусерстате](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[Девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Чтение свойств и связей объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Создание Девицеманажементинтентусерстате](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[Девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Создание нового объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Удаление Девицеманажементинтентусерстате](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|Нет|Удаляет объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md).|
|[Обновление Девицеманажементинтентусерстате](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[Девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Обновление свойств объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор|
|userPrincipalName|String|Имя участника-пользователя, сообщаемое на устройстве|
|userName|String|Имя пользователя, сообщаемое на устройстве|
|deviceCount|Int32|Количество устройств, принадлежащие пользователю для намерения|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о намерениях|
|state|[Комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние пользователя для намерения. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|

## <a name="relationships"></a>Отношения
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







