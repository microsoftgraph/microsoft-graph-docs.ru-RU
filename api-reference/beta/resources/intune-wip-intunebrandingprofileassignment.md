---
title: Тип ресурса Интунебрандингпрофилеассигнмент
description: Эта сущность содержит свойства, используемые для назначения профиля фирменной символики группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc3e7442202c9d6de3bab5dd19d536a528bdfc85
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763279"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>Тип ресурса Интунебрандингпрофилеассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения профиля фирменной символики группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Интунебрандингпрофилеассигнментс](../api/intune-wip-intunebrandingprofileassignment-list.md)|Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Список свойств и связей объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Получение Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-get.md)|[интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Чтение свойств и связей объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Создание Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-create.md)|[интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Удаление Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Нет|Удаляет объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Обновление Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-update.md)|[интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, которой назначен профиль фирменной символики.|

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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



