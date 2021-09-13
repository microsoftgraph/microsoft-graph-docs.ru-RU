---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd5720a577d8f45b22d146648a7ab205b2b38c17
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111336"
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



