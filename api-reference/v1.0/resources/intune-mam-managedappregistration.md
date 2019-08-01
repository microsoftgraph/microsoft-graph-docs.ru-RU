---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a7b10a7d960c449aee4f911f4992955bde18724
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037914"
---
# <a name="managedappregistration-resource-type"></a>Тип ресурса managedAppRegistration

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppRegistration](../api/intune-mam-managedappregistration-list.md)|Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Получение объекта managedAppRegistration](../api/intune-mam-managedappregistration-get.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Функция getUserIdsWithFlaggedAppRegistration](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|Коллекция объектов string|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления.|
|applicationVersion|String|Версия приложения.|
|managementSdkVersion|String|Версия пакета SDK для управления приложениями.|
|platformVersion|String|Версия операционной системы.|
|deviceType|String|Тип главного устройства.|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях.|
|deviceName|String|Имя главного устройства.|
|flaggedReasons|Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)|Нуль или более причин, по которым помечается регистрация приложения например приложения, запущенного на устройстве с административным доступом.|
|userId|String|ИД пользователя, к которому относится эта регистрация приложения.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения.|
|id|Строка|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.|
|intendedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, которые на текущий момент администратор использует для приложения.|
|operations|Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Нуль или более долговременных операций, запускаемых для регистрации приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


