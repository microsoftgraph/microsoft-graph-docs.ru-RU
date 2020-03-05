---
title: Тип ресурса К mobileappprovisioningconfiggroupassignment.
description: Содержит свойства, используемые для назначения конфигурации подготовки приложений группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b912c55b6b0f526246938356bc913da9e8717b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491479"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a>Тип ресурса К mobileappprovisioningconfiggroupassignment.

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения конфигурации подготовки приложений группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеапппровисионингконфигграупассигнментс](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|Коллекция [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Список свойств и связей объектов [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Получение К mobileappprovisioningconfiggroupassignment.](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Чтение свойств и связей объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Создание К mobileappprovisioningconfiggroupassignment.](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Создание нового объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|
|[Удаление К mobileappprovisioningconfiggroupassignment.](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|Нет|Удаляет объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).|
|[Обновление К mobileappprovisioningconfiggroupassignment.](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md);|Обновление свойств объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|таржетграупид|String|Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.|
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



