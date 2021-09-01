---
title: termsAndConditionsGroupAssignment type
description: Объект termsAndConditionsGroupAssignment представляет назначение данной политики терминов и условий (T&C) данной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c92a30d44c2f87e74e5f7c2d0b5ae3a83bc09a02
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785187"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>termsAndConditionsGroupAssignment type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект termsAndConditionsGroupAssignment представляет назначение данной политики терминов и условий (T&C) данной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Условия спискаAndConditionsGroupAssignments](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection|Список свойств и связей объектов [TermsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Get termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Чтение свойств и связей объекта [TermsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Создание терминовAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Создайте новый [объект TermsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Удаление терминовAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|Нет|Удаляет [терминAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).|
|[Update termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Обновление свойств объекта [termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|targetGroupId|Строка|Уникальный идентификатор группы, для&C.|

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



