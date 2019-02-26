---
title: Тип ресурса Термсандкондитионсграупассигнмент
description: Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (Т_амп_к) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5b97e691ff16ce2c86057ab5dae229d8657974
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142688"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>Тип ресурса Термсандкондитионсграупассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (Т_амп_к) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Термсандкондитионсграупассигнментс](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|Коллекция [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Список свойств и связей объектов [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Получение Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[Термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Чтение свойств и связей объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Создание Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[Термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Удаление Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|Нет|Удаляет объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md).|
|[Обновление Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[Термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Обновление свойств объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|Таржетграупид|String|Уникальный идентификатор группы, которой назначена политика Т_амп_к.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Ссылка для перехода к назначенным условиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




