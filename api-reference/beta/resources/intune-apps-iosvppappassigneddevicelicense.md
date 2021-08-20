---
title: тип ресурса iosVppAppAssignedDeviceLicense
description: Назначение лицензии на устройство программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf0a15038d1b848d52f3779d469edd0a42e6e797d9c1419ee7158076f97fc8f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226548"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>тип ресурса iosVppAppAssignedDeviceLicense

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии на устройство программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.


Наследует [от iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosVppAppAssignedDeviceLicenses](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|[коллекция iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Список свойств и связей объектов [iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)|
|[Get iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Чтение свойств и связей объекта [iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)|
|[Создание iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Создайте новый [объект iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)|
|[Удаление iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|Нет|Удаляет [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).|
|[Обновление iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Обновление свойств объекта [iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|String|Адрес электронной почты пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|Имя участника-пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|managedDeviceId|Строка|ID управляемого устройства.|
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




