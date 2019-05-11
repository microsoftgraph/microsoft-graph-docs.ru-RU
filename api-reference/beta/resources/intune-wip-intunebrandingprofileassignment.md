---
title: Тип ресурса Интунебрандингпрофилеассигнмент
description: Эта сущность содержит свойства, используемые для назначения профиля фирменной символики группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c3b27c0fe42b0fe1bc3b3350bc98957e88e92b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939765"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>Тип ресурса Интунебрандингпрофилеассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения профиля фирменной символики группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Интунебрандингпрофилеассигнментс](../api/intune-wip-intunebrandingprofileassignment-list.md)|Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Список свойств и связей объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Получение Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-get.md)|[Интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Чтение свойств и связей объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Создание Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-create.md)|[Интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|
|[Удаление Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Нет|Удаляет объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[Обновление Интунебрандингпрофилеассигнмент](../api/intune-wip-intunebrandingprofileassignment-update.md)|[Интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта.|
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




