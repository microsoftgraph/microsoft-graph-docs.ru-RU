---
title: Тип ресурса iosVppAppAssignedDeviceLicense
description: операций ввода-вывода устройства программа покупки корпоративного лицензионного назначения. Этот класс не поддерживает операции создания, удаления и обновления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b18415b3a2d25990bc7202d96fc35f3289b56f4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393615"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>Тип ресурса iosVppAppAssignedDeviceLicense

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

операций ввода-вывода устройства программа покупки корпоративного лицензионного назначения. Этот класс не поддерживает операции создания, удаления и обновления.


Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosVppAppAssignedDeviceLicenses](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) коллекции|Свойства списка и связей объектов [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Получение iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Чтение свойства и связи объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Создание iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Создание нового объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Удаление iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|Нет|Удаляет [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).|
|[Обновление iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Обновление свойства объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|String|Адрес электронной почты пользователя. Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|Имя участника-пользователя. Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|managedDeviceId|String|С идентификатором управляемого устройства.|
|deviceName|String|Имя устройства.|

## <a name="relationships"></a>Отношения
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




