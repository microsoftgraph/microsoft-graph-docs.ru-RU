---
title: Тип ресурса Иосвппаппассигнеддевицелиценсе
description: Назначение лицензии на устройство для корпоративного приобретения для iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffee75852896b6657fa7af726d7ac014ae2b8d07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493407"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>Тип ресурса Иосвппаппассигнеддевицелиценсе

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии на устройство для корпоративного приобретения для iOS. Этот класс не поддерживает операции создания, удаления и обновления.


Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосвппаппассигнеддевицелиценсес](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|Коллекция [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Список свойств и связей объектов [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Получение Иосвппаппассигнеддевицелиценсе](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Чтение свойств и связей объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Создание Иосвппаппассигнеддевицелиценсе](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Создание нового объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Удаление Иосвппаппассигнеддевицелиценсе](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|Нет|Удаляет объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md).|
|[Обновление Иосвппаппассигнеддевицелиценсе](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Обновление свойств объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|усеремаиладдресс|String|Адрес электронной почты пользователя. Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|Строка|Имя участника-пользователя. Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|манажеддевицеид|String|Идентификатор управляемого устройства.|
|deviceName|String|Имя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedDeviceLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "managedDeviceId": "String",
  "deviceName": "String"
}
```



