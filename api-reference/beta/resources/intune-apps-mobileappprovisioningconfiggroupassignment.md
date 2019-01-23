---
title: Тип ресурса mobileAppProvisioningConfigGroupAssignment
description: Содержит свойства, используемые для назначения к конфигурации подготовки приложения в группу.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ad07112031ce8ebe46d48c2c5fa51f0744a2bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421930"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a>Тип ресурса mobileAppProvisioningConfigGroupAssignment

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения к конфигурации подготовки приложения в группу.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppProvisioningConfigGroupAssignments](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) коллекции|Свойства списка и связей объектов [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Получение mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Чтение свойства и связи объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Создание mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Создание нового объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Удаление mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|Нет|Удаляет [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).|
|[Обновление mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Обновление свойства объекта [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|targetGroupId|String|Идентификатор группы AAD целевого приложения подготовки конфигурации.|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```




