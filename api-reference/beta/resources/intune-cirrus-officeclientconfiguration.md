---
title: тип ресурса officeClientConfiguration
description: Office Конфигурация клиента.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cacf0d4624b984e02a4051d9b8b166ecece7a38e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127516"
---
# <a name="officeclientconfiguration-resource-type"></a>тип ресурса officeClientConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Office Конфигурация клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|[коллекция officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Список свойств и связей объектов [officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)|
|[Получить officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Чтение свойств и связей объекта [officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)|
|[Действие assign](../api/intune-cirrus-officeclientconfiguration-assign.md)|[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Замените все целевые группы для политики.|
|[Действие updatePriorities](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Нет|Обновление приоритетов политики.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id политики конфигурации клиента office.|
|userPreferencePayload|Stream|Параметры параметров JSON строки в двоичном формате, эти значения могут быть переопределены пользователем.|
|policyPayload|Stream|Параметры JSON строки JSON в двоичном формате, эти значения не могут быть изменены пользователем.|
|description|String|Пока не задокументировано.|
|displayName|String|Администратор предоставил описание политики конфигурации клиента office.|
|lastModifiedDateTime|Даты и время|Последний измененный штамп даты политики.|
|priority|Int32|Значение приоритета должно быть уникальным значением для каждой политики клиента и использоваться для разрешения конфликтов, более низкие значения означают высокий приоритет.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сводка регистрации пользователя для политики.|
|checkinStatuses|[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния регистрации клиента office.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список групповых назначений для политики.|

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



