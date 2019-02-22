---
title: Тип ресурса Интунебрандингпрофилеассигнмент
description: Эта сущность содержит свойства, используемые для назначения профиля фирменной символики группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 956cf652167714270dfcaf348523db236fb62941
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151396"
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
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, которой назначен профиль фирменной символики.|

## <a name="relationships"></a>Отношения
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




