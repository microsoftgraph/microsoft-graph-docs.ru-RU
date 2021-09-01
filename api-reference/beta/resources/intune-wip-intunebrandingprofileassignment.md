---
title: тип ресурса intuneBrandingProfileAssignment
description: Эта сущность содержит свойства, используемые для назначения профиля брендинга группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f974c936e8b5c3ad39abfdaaf37a5a3e69bee150
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797467"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>тип ресурса intuneBrandingProfileAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения профиля брендинга группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[коллекция intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Список свойств и связей объектов [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Получить intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Чтение свойств и связей объекта [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Создание intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Создайте новый [объект intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|
|[Удаление intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Нет|Удаляет [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Обновление intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Обновление свойств объекта [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Назначение цели, назначенной профилем брендинга.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



