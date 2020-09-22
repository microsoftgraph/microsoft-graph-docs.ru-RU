---
title: Тип ресурса Термсандкондитионсграупассигнмент
description: Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (T&C) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29cc8d853c9cb9bf426544681a9e69a0f4e4a5ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024376"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>Тип ресурса Термсандкондитионсграупассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (T&C) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Термсандкондитионсграупассигнментс](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|Коллекция [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Список свойств и связей объектов [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Получение Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Чтение свойств и связей объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Создание Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Удаление Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|Нет|Удаляет объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md).|
|[Обновление Термсандкондитионсграупассигнмент](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Обновление свойств объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|таржетграупид|String|Уникальный идентификатор группы, которой назначена политика T&C.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
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






