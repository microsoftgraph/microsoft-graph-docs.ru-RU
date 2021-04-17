---
title: Тип ресурса identityUserFlowAttribute
description: Представляет атрибуты потоков пользователей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: ca8930a5cb11edb1cf7345464666478cfc01bcda
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882602"
---
# <a name="identityuserflowattribute-resource-type"></a>Тип ресурса identityUserFlowAttribute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет атрибуты потоков пользователей в клиенте Azure Active Directory (Azure AD) и клиенте Azure AD B2C.

Настройка атрибутов потоков пользователей в клиенте Azure AD или Azure AD B2C позволяет вам собирать сведения о пользователе во время регистрации. Вы можете выбрать сбор встроенного набора атрибутов, например имени, фамилии, города и почтового индекса. Кроме того, вы можете настроить специальные атрибуты потоков пользователей для сбора сведений о пользователе, которые не встроены в каталог. Настраиваемые атрибуты потоков пользователей — это абстрагирование от [расширений схемы Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).

[identityBuiltInUserFlowAttributes](../resources/identitybuiltinuserflowattribute.md) и [identityCustomUserFlowAttributes](../resources/identitycustomuserflowattribute.md) наследуются от этого базового типа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityuserflowattribute-list.md)|identityUserFlowAttributes collection|Извлечение всех встроенных и настраиваемых атрибутов потоков пользователей.|
|[Создание](../api/identityuserflowattribute-post.md)|identityUserFlowAttribute|Создание настраиваемого атрибута потока пользователей.|
|[Получение](../api/identityuserflowattribute-get.md) |identityUserFlowAttribute|Извлечение свойств атрибута потока пользователей.|
|[Обновление](../api/identityuserflowattribute-update.md)|Нет|Обновление настраиваемого атрибута потока пользователей.|
|[удаление](../api/identityuserflowattribute-delete.md);|Нет|Удаление настраиваемого атрибута потока пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор атрибута потока пользователей. Это автоматически созданный атрибут только для чтения.|
|displayName|String|Отображаемое имя атрибута потока пользователей.|
|description|String|Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.|
|userFlowAttributeType|identityUserFlowAttributeType|Тип атрибута потока пользователей. Это автоматически настроенный атрибут только для чтения. В зависимости от типа атрибута значением этого свойства является `builtIn`, `custom` или `required`.|
|dataType|identityUserFlowAttributeDataType|Тип данных атрибута потока пользователей. Это свойство нельзя изменить после создания атрибута потока пользователей. Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
