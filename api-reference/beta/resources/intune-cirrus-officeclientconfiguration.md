---
title: Тип ресурса officeClientConfiguration
description: Настройка клиента Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fabc35866aafbbb4052ce5eab3f0de977ec6adb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488539"
---
# <a name="officeclientconfiguration-resource-type"></a>Тип ресурса officeClientConfiguration

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка клиента Office.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Оффицеклиентконфигуратионс](../api/intune-cirrus-officeclientconfiguration-list.md)|Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Список свойств и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[Получение officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Чтение свойств и связей объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[Действие assign](../api/intune-cirrus-officeclientconfiguration-assign.md)|Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Замените все целевые группы для политики.|
|[Действие updatePriorities](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Нет|Обновление приоритетов политики.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики конфигурации клиента Office.|
|усерпреференцепайлоад|Stream|Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.|
|полиципайлоад|Stream|Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.|
|description|String|Пока не задокументировано.|
|displayName|Строка|Администратор предоставил описание политики конфигурации клиента Office.|
|lastModifiedDateTime|DateTime|Метка даты и времени последнего изменения политики.|
|priority|Int32|Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.|
|усерчеккинсуммари|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сводка по возврату пользователя для политики.|
|чеккинстатусес|Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния возврата клиента Office.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список назначений групп для политики.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



