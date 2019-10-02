---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 15fca0cedc6fe1da81da25688bbc447c1f8f475f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360106"
---
# <a name="user-resource-type"></a>Тип ресурса user

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет объект пользователя Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов Users](../api/intune-shared-user-list.md) .|Коллекция объектов [user](../resources/intune-shared-user.md)|Список свойств и связей объектов [user](../resources/intune-shared-user.md).|
|[Получение объекта User](../api/intune-shared-user-get.md) .|Коллекция объектов [user](../resources/intune-shared-user.md)|Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).|
|[Создание объекта User](../api/intune-shared-user-create.md) .|Коллекция объектов [user](../resources/intune-shared-user.md)|Создание объекта [user](../resources/intune-shared-user.md).|
|[Удаление пользователя](../api/intune-shared-user-delete.md).|Нет|Удаляет объект [user](../resources/intune-shared-user.md).|
|[Обновление объекта пользователя](../api/intune-shared-user-update.md) .|[user](../resources/intune-shared-user.md)|Обновление свойств объекта [user](../resources/intune-shared-user.md).|
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
|**Входящая миграция**|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|


## <a name="relationships"></a>Связи
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

