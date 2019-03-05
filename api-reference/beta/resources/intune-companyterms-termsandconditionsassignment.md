---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 309136805a6d5e41a5aee8e20cc80b6d7665ef66
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156065"
---
# <a name="termsandconditionsassignment-resource-type"></a>Тип ресурса termsAndConditionsAssignment

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список termsAndConditionsAssignments](../api/intune-companyterms-termsandconditionsassignment-list.md)|Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Получение объекта termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Создание объекта termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-create.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Удаление объекта termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-delete.md)|Нет|Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Обновление объекта termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-update.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Объект, для которого назначается политика соблюдения условий.|

## <a name="relationships"></a>Связи
None

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




