---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f486e3202535882d719e5f6c083b583321e917b5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732801"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет объект пользователя Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов](../api/intune-shared-user-list.md) пользователей.|Коллекция объектов [user](../resources/intune-shared-user.md)|Список свойств и связей объектов [user](../resources/intune-shared-user.md).|
|[Получите объект](../api/intune-shared-user-get.md) пользователя.|Коллекция объектов [user](../resources/intune-shared-user.md)|Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).|
|[Создание объекта](../api/intune-shared-user-create.md) пользователя.|Коллекция объектов [user](../resources/intune-shared-user.md)|Создание объекта [user](../resources/intune-shared-user.md).|
|[Удаление пользователя](../api/intune-shared-user-delete.md).|Нет|Удаляет объект [user](../resources/intune-shared-user.md).|
|[Обновление объекта](../api/intune-shared-user-update.md) пользователя.|[user](../resources/intune-shared-user.md)|Обновление свойств объекта [user](../resources/intune-shared-user.md).|
|**Управление устройствами**|
|[Действие removeAllDevicesFromManagement](../api/intune-shared-user-removealldevicesfrommanagement.md)|Нет|Прекращение управления всеми устройствами для этого пользователя|
|**Управление мобильным приложением (MAM)**|
|[Функция getManagedAppDiagnosticStatuses](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Получает состояние диагностической проверки определенного пользователя.|
|[Функция getManagedAppPolicies](../api/intune-shared-user-getmanagedapppolicies.md)|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Получает ограничения приложений для определенного пользователя.|
|[Действие wipeManagedAppRegistrationsByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|
|**Адаптация**|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|


## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Управляемые устройства, связанные с пользователем.|
|**Управление мобильным приложением (MAM)**|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.|
|**Устранение неполадок**|
|deviceManagementTroubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для этого пользователя.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->






