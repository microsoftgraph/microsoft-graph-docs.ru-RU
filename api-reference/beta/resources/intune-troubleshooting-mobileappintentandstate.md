---
title: тип ресурса mobileAppIntentAndState
description: Намерение MobileApp и установка состояния для данного устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40d555aacab29757622bb6e82d5358eb0c89ed42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023264"
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




