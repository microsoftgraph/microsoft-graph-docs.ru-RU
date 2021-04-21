---
title: Обновление identityUserFlowAttributeAssignment
description: Обновление свойств объекта userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d0835b4f3c3fc24496cdde75ddb9d6684691c600
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920611"
---
# <a name="update-identityuserflowattributeassignment"></a>Обновление identityUserFlowAttributeAssignment

Пространство имен: microsoft.graph

Обновление свойств объекта identityUserFlowAttributeAssignment.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|IdentityUserFlow.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса подарят представление JSON объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

В следующей таблице показаны свойства, доступные для обновления в [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени identityUserFlowAttribute в потоке пользователей.|
|isOptional|Boolean|Определяет, является ли identityUserFlowAttribute необязательным. `true` означает, что пользователю не нужно предоставлять значение. `false` означает, что пользователь не может выполнить регистрацию без предоставления значения.|
|requiresVerification|Boolean|Определяет, требуется ли проверка identityUserFlowAttribute. Это используется только для проверки номера телефона или адреса электронной почты пользователя.|
|userAttributeValues|[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)|Параметры ввода атрибута потока пользователя. Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|Тип ввода атрибута потока пользователя. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userattributeassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userattributeassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userattributeassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userattributeassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
