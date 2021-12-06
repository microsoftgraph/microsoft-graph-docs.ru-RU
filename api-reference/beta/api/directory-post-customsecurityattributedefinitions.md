---
title: Создание customSecurityAttributeDefinition
description: Создайте новый объект customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b7f49cbddc27a3681882fa9756ff0b46dd2fdb8f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226804"
---
# <a name="create-customsecurityattributedefinition"></a>Создание customSecurityAttributeDefinition
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|CustomSecAttributeDefinition.ReadWrite.All|

Пользователю, заявляемого в службу, также необходимо уписать администратору определения атрибутов [роль каталога](/azure/active-directory/roles/permissions-reference. По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/customSecurityAttributeDefinitions
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса подарят представление JSON объекта [customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)

В следующей таблице показаны свойства, которые можно настроить при создании [customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|attributeSet|Строка|Имя набора атрибутов. Случай нечувствительный. Обязательный.|
|description|Строка|Описание настраиваемого атрибута безопасности. Может иметь длину до 128 символов и включать символы Unicode. Не может содержать пробелы или специальные символы. Можно изменить позже. Необязательный параметр.|
|isCollection|Логическое|Указывает, можно ли наказать несколько значений к настраиваемой атрибуту безопасности. Не удается изменить позже. Если `type` задана настройка Boolean, `isCollection` не может быть задана истина. Обязательный.|
|isSearchable|Boolean|Указывает, будут ли индексироваться пользовательские значения атрибутов безопасности для поиска объектов, за которые назначены значения атрибутов. Не удается изменить позже. Обязательный.|
|name|String|Имя настраиваемого атрибута безопасности. Должно быть уникальным в наборе атрибутов. Может иметь длину до 32 символов и включать символы Unicode. Не может содержать пробелы или специальные символы. Не удается изменить позже. Случай нечувствительный. Обязательный.|
|status|String|Указывает, активен ли настраиваемый атрибут безопасности или отключен. Допустимые значения `Available` и `Deprecated` . Можно изменить позже. Обязательное.|
|type|Строка|Тип данных для пользовательских значений атрибута безопасности. Поддерживаемые типы `Boolean` , `Integer` и `String` . Не удается изменить позже. Обязательный.|
|usePreDefinedValuesOnly|Логическое|Указывает, могут ли быть назначены только предопределяемые значения атрибуту настраиваемой безопасности. Если установлено значение false, разрешены значения свободной формы. Позже может быть изменено с true на false, но не может быть изменено с false на true. Если `type` задана настройка Boolean, `usePreDefinedValuesOnly` не может быть задана истина. Обязательный.|

Свойство `id` автогенерировано и не может быть установлено.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и настраиваемый `201 Created` [объектSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-a-custom-security-attribute"></a>Пример 1. Добавление настраиваемой атрибута безопасности

В следующем примере добавляется новое пользовательское определение атрибута безопасности, которое является одним свободным значением типа String.

+ Набор атрибутов: `Engineering`
+ Атрибут: `ProjectDate`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json

{
    "attributeSet":"Engineering",
    "description":"Target completion date",
    "isCollection":false,
    "isSearchable":true,
    "name":"ProjectDate",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Target completion date",
    "id": "Engineering_ProjectDate",
    "isCollection": false,
    "isSearchable": true,
    "name": "ProjectDate",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": false
}
```

### <a name="example-2-add-a-custom-security-attribute-that-supports-multiple-predefined-values"></a>Пример 2. Добавьте настраиваемый атрибут безопасности, который поддерживает несколько предопределяемых значений

В следующем примере добавляется новое настраиваемого определения атрибута безопасности, которое поддерживает несколько значений типа String, заранее задав.

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition_v2"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json
Content-length: 310

{
    "attributeSet":"Engineering",
    "description":"Active projects for user",
    "isCollection":true,
    "isSearchable":true,
    "name":"Project",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-customsecurityattributedefinition-v2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-customsecurityattributedefinition-v2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-customsecurityattributedefinition-v2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-customsecurityattributedefinition-v2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-customsecurityattributedefinition-v2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Active projects for user",
    "id": "Engineering_Project",
    "isCollection": true,
    "isSearchable": true,
    "name": "Project",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": true
}
```
