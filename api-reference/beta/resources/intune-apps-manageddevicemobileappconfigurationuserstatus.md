---
title: Тип ресурса managedDeviceMobileAppConfigurationUserStatus
description: Содержит свойства, унаследованные свойства и действия состояния конфигурации мобильных приложений MDM для пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd2f0a697f8535d07afb9d30d11efed315941d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552144"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationUserStatus

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, унаследованные свойства и действия состояния конфигурации мобильных приложений MDM для пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Получение объекта managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Создание объекта managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Удаление объекта managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|Нет|Удаляет объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Обновление объекта managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userDisplayName|String|Имя пользователя в объекте DevicePolicyStatus.|
|devicesCount|Int32|Количество устройств для этого пользователя.|
|status|[Комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





