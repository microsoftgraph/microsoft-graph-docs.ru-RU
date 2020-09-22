---
title: Тип ресурса Мобилеаппинтентандстате
description: MobileApp намерения и состояние установки для конкретного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4c8e94599c78c82efab6051a58043ac96be5326
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003586"
---
# <a name="mobileappintentandstate-resource-type"></a>Тип ресурса Мобилеаппинтентандстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

MobileApp намерения и состояние установки для конкретного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеаппинтентандстатес](../api/intune-troubleshooting-mobileappintentandstate-list.md)|Коллекция [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md)|Список свойств и связей объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Получение Мобилеаппинтентандстате](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Чтение свойств и связей объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Создание Мобилеаппинтентандстате](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Создание нового объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Удаление Мобилеаппинтентандстате](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Нет|Удаляет объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[Обновление Мобилеаппинтентандстате](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md);|Обновление свойств объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|мобилеапплист|Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|Список целей и состояний полезных данных для клиента.|

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






