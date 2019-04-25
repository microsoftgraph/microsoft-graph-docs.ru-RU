---
title: Тип ресурса Виндовсоффицеклиентконфигуратион
description: Объект, описывающий параметры политики Office для Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61b64b53fb5a4000b0e8c5366c5a821c6941ce61
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526344"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a>Тип ресурса Виндовсоффицеклиентконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, описывающий параметры политики Office для Windows.

НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсоффицеклиентконфигуратионс](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|Коллекция [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Список свойств и связей объектов [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Получение Виндовсоффицеклиентконфигуратион](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Чтение свойств и связей объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Создание Виндовсоффицеклиентконфигуратион](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Создание нового объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Удаление Виндовсоффицеклиентконфигуратион](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|Нет|Удаляет объект [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md).|
|[Обновление Виндовсоффицеклиентконфигуратион](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Обновление свойств объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор политики конфигурации клиента Office. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Усерпреференцепайлоад|Поток|Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Полиципайлоад|Поток|Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|String|Администратор предоставил описание политики конфигурации клиента Office. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|String|Предоставленное администратором имя политики конфигурации клиента Office. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|priority|Int32|Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Метка даты и времени последнего изменения политики. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Усерчеккинсуммари|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сводка по возврату пользователя для политики. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Чеккинстатусес|Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния возврата клиента Office. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список назначений групп для политики. НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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



