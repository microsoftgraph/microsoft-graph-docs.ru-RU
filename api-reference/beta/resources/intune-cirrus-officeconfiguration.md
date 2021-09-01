---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58e1aea2e6b8a03f69e63948675e4f4b7a9b6ebf
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820529"
---
# <a name="officeconfiguration-resource-type"></a>Тип ресурса officeConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|Get officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Чтение свойств и связей [объекта OfficeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)|
|Обновление officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Обновление свойств объекта [officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id конфигурации офиса.|
|tenantCheckinStatuses|[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния регистрации клиента office.|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Объект, описывая статуи регистрации клиента|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|clientConfigurations|[коллекция officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Список конфигурации клиента office.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
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
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



