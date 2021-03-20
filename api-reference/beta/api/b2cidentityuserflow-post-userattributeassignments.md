---
title: Создание userAttributeAssignments
description: Создайте новый объект identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52e459d65820ca1225e5aefe2eafff0f5a044ecc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944693"
---
# <a name="create-userattributeassignments"></a>Создание userAttributeAssignments

Пространство имен: microsoft.graph

Создайте новый объект identityUserFlowAttributeAssignment в [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|IdentityUserFlow.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса подарят представление JSON объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

В следующей таблице показаны свойства, необходимые при создании [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени identityUserFlowAttribute в потоке пользователей.|
|isOptional|Boolean|Определяет, является ли identityUserFlowAttribute необязательным. `true` означает, что пользователю не нужно предоставлять значение. `false` означает, что пользователь не может завершить регистрацию без предоставления значения.|
|requiresVerification|Boolean|Определяет, требуется ли проверка identityUserFlowAttribute. Это используется только для проверки номера телефона или адреса электронной почты пользователя.|
|userAttributeValues|[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)|Параметры ввода атрибута потока пользователя. Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|Тип ввода атрибута потока пользователя. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|Идентификатор атрибута потока пользователей, который должен включаться в назначение потока пользователей.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2C_1_Consumer/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
