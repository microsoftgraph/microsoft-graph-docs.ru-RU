---
title: тип ресурса mobileAppIntentAndState
description: Намерение MobileApp и установка состояния для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8e5b3c8eb1e221adffcd79f65884c688067d1ba
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255942"
---
# <a name="mobileappintentandstate-resource-type"></a>тип ресурса mobileAppIntentAndState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Намерение MobileApp и установка состояния для данного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[коллекция mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Список свойств и связей объектов [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Get mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Чтение свойств и связей объекта [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Создание mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Создание нового [объекта mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Удаление mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Нет|Удаляет [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[Обновление mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Обновление свойств объекта [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|mobileAppList|[коллекция mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|Список намерений и состояния полезной нагрузки для клиента.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```




