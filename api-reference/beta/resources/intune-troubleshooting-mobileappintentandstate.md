---
title: Тип ресурса Мобилеаппинтентандстате
description: MobileApp намерения и состояние установки для конкретного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bc39ec4db3c777fc7cf34528e9d8054f6d382e8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939772"
---
# <a name="mobileappintentandstate-resource-type"></a>Тип ресурса Мобилеаппинтентандстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|UUID объекта.|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|Мобилеапплист|Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|Список целей и состояний полезных данных для клиента.|

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




