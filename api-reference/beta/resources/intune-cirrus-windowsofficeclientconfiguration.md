---
title: тип ресурса windowsOfficeClientConfiguration
description: Объект, описывая параметры политики office для Windows.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 542effabbd82a000c02e1da5e86705532c11bbb2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101872"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a>тип ресурса windowsOfficeClientConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, описывая параметры политики office для Windows.

Наследуется [от officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsOfficeClientConfigurations](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|[коллекция windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Список свойств и связей [объектов WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|
|[Получить windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Чтение свойств и связей объекта [WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|
|[Создание windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Создайте [новый объект WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|
|[Удаление windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|Нет|Удаляет [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).|
|[Обновление windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Обновление свойств объекта [WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id политики конфигурации клиента office. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|Параметры параметров JSON строки в двоичном формате, эти значения могут быть переопределены пользователем. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|Параметры JSON строки JSON в двоичном формате, эти значения не могут быть изменены пользователем. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|String|Администратор предоставил описание политики конфигурации клиента office. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|String|Администратор предоставил имя политики конфигурации клиента office. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|priority|Int32|Значение приоритета должно быть уникальным значением для каждой политики клиента и использоваться для разрешения конфликтов, более низкие значения означают высокий приоритет. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|Даты и время|Последний измененный штамп даты политики. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сводка регистрации пользователя для политики. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния регистрации клиента office. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список групповых назначений для политики. Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

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



