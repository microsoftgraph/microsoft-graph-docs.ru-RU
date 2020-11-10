---
title: Создание Идентитюсерфловаттрибуте
description: Создание нового объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 816b9e94ca95ec61f7a9628de7ede6617cebb7fd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953144"
---
# <a name="create-identityuserflowattribute"></a>Создание Идентитюсерфловаттрибуте

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|IdentityUserFlow.ReadWrite.All|

Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:

* Глобальный администратор
* Администратор атрибутов пользовательского процесса внешнего удостоверения

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте представление объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)в формате JSON.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор атрибута потока пользователей. Это автоматически созданный атрибут только для чтения.|
|displayName|String|Отображаемое имя атрибута потока пользователей.|
|description|String|Описание атрибута Flow User. Он отображается для пользователя во время регистрации.|
|userFlowAttributeType|String|Тип атрибута потока пользователей. Это автоматически настроенный атрибут только для чтения. В зависимости от типа атрибута значением этого свойства является `builtIn` или `custom`.|
|dataType|String|Тип данных атрибута потока пользователей. Этот параметр нельзя изменить после создания настраиваемого атрибута пользовательского процесса. Поддерживаемые значения для **dataType** :<br/><ul><li>`string` : указывает, что тип данных для Идентитюсерфловаттрибуте является строкой. </li><li>`boolean` : указывает, что тип данных для Идентитюсерфловаттрибуте является логическим.</li><li>`int64` : указывает, что тип данных для Идентитюсерфловаттрибуте является целым числом.</li></ul>|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) в тексте отклика. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
