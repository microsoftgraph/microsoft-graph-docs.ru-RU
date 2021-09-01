---
title: тип ресурсов securityBaselineDeviceState
description: Сводка базового состояния соответствия требованиям безопасности базового уровня безопасности для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99dae7127ff0074fd660ed90bf0467fc8e6f5986
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805733"
---
# <a name="securitybaselinedevicestate-resource-type"></a>тип ресурсов securityBaselineDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка базового состояния соответствия требованиям безопасности базового уровня безопасности для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список securityBaselineDeviceStates](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|[коллекция securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Список свойств и связей объектов [securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Get securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Чтение свойств и связей объекта [securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Создание securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Создайте новый [объект securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Удаление securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|Нет|Удаляет [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).|
|[Обновление securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Обновление свойств объекта [securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор сущности|
|managedDeviceId|Строка|ID устройства Intune|
|deviceDisplayName|String|Отображение имени устройства|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Состояние соответствия базовым требованиям безопасности. Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|lastReportedDateTime|DateTimeOffset|Последнее измененное время даты отчета о политике|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```



