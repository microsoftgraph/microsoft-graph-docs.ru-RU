---
title: тип ресурса windowsDriverUpdateInventory
description: Новая сущность для представления запасов драйвера.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06fa58d5e4428e55e0d76a37c484519c566198d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029936"
---
# <a name="windowsdriverupdateinventory-resource-type"></a>тип ресурса windowsDriverUpdateInventory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Новая сущность для представления запасов драйвера.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsDriverUpdateInventories](../api/intune-softwareupdate-windowsdriverupdateinventory-list.md)|[коллекция windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Список свойств и связей [объектов WindowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Получить windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-get.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Чтение свойств и связей [объекта WindowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Создание windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-create.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Создание нового [объекта WindowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Удаление windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-delete.md)|Нет|Удаляет [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md).|
|[Обновление windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-update.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Обновление свойств объекта [WindowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID драйвера.|
|name|String|Имя водителя.|
|version|String|Версия драйвера.|
|manufacturer|String|Производитель драйвера.|
|releaseDateTime|DateTimeOffset|Время выпуска драйвера.|
|driverClass|Строка|Класс драйвера.|
|applicableDeviceCount|Int32|Количество устройств, для которых применим этот драйвер.|
|approvalStatus|[driverApprovalStatus](../resources/intune-softwareupdate-driverapprovalstatus.md)|Состояние утверждения для этого драйвера. Возможные значения: `needsReview`, `declined`, `approved`, `suspended`.|
|category|[driverCategory](../resources/intune-softwareupdate-drivercategory.md)|Категория для этого драйвера. Возможные значения: `recommended`, `previouslyApproved`, `other`.|
|deployDateTime|DateTimeOffset|Дата развертывания драйвера при утвержденииStatus.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateInventory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "id": "String (identifier)",
  "name": "String",
  "version": "String",
  "manufacturer": "String",
  "releaseDateTime": "String (timestamp)",
  "driverClass": "String",
  "applicableDeviceCount": 1024,
  "approvalStatus": "String",
  "category": "String",
  "deployDateTime": "String (timestamp)"
}
```



