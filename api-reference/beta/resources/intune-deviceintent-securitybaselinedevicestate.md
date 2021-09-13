---
title: тип ресурсов securityBaselineDeviceState
description: Сводка базового состояния соответствия требованиям безопасности базового уровня безопасности для устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f960ec9f9a0b56b8a28cda555cf78514cebb0bbb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051253"
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
|managedDeviceId|String|ID устройства Intune|
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



