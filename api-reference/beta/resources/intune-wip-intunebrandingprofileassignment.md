---
title: тип ресурса intuneBrandingProfileAssignment
description: Эта сущность содержит свойства, используемые для назначения профиля брендинга группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d97eda1fc92ca5979f1712821d5fbc30229a23db0943860b0386a7d1d212d48e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209765"
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




