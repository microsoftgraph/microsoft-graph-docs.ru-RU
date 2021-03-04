---
title: Тип ресурса identityUserFlowAttribute
description: Представляет атрибуты потоков пользователей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 3e8707627b09784972a1a578fe4b6b84a623f4dd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440244"
---
# <a name="identityuserflowattribute-resource-type"></a>Тип ресурса identityUserFlowAttribute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет атрибуты потоков пользователей в клиенте Azure Active Directory (Azure AD) и клиенте Azure AD B2C.

Настройка атрибутов потоков пользователей в клиенте Azure AD или Azure AD B2C позволяет вам собирать сведения о пользователе во время регистрации. Вы можете выбрать сбор встроенного набора атрибутов, например имени, фамилии, города и почтового индекса. Кроме того, вы можете настроить специальные атрибуты потоков пользователей для сбора сведений о пользователе, которые не встроены в каталог. Настраиваемые атрибуты потоков пользователей — это абстрагирование от [расширений схемы Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).

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
|userFlowAttributeType|String|Тип атрибута потока пользователей. Это автоматически настроенный атрибут только для чтения. В зависимости от типа атрибута значением этого свойства является `builtIn` или `custom`.|
|dataType|String|Тип данных атрибута потока пользователей. Это свойство нельзя изменить после создания атрибута потока пользователей. Поддерживаемые значения для **dataType**:<br/><ul><li>`string` — указывает, что dataType для identityUserFlowAttribute является строкой. </li><li>`boolean` — указывает, что dataType для identityUserFlowAttribute является логическим значением.</li><li>`int64` — указывает, что dataType для identityUserFlowAttribute является целым числом.</li></ul>|

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
