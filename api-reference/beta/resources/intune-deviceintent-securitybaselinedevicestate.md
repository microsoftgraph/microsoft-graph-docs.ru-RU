---
title: тип ресурсов securityBaselineDeviceState
description: Сводка базового состояния соответствия требованиям безопасности базового уровня безопасности для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da4dcad2cd0f8956f43e4322b166495576432d751324b642e867c06df1cb76a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224679"
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
|id|String|Уникальный идентификатор сущности|
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




