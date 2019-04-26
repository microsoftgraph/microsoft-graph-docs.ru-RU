---
title: Тип ресурса Мобилеаппинтентандстате
description: MobileApp намерения и состояние установки для конкретного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e90251338ad7e740b216452a52cc0fffcfc44565
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558155"
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
|id|String|UUID объекта.|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|Мобилеапплист|Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|Список целей и состояний полезных данных для клиента.|

## <a name="relationships"></a>Отношения
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



