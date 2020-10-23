---
title: Тип ресурса Термсандкондитионсграупассигнмент
description: Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (T&C) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9236ee34c07836e97fca89636f128b12dbb7d576
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726516"
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
|id|Строка|Уникальный идентификатор объекта.|
|таржетграупид|Строка|Уникальный идентификатор группы, которой назначена политика T&C.|

## <a name="relationships"></a>Связи
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





