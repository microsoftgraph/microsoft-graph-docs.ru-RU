---
title: Создание Фонеаусентикатионмесод
description: Добавление нового метода проверки подлинности телефона.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bd29ee6e2f78e8864bce6a09cac456c4ab5ce6a
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429593"
---
# <a name="create-phoneauthenticationmethod"></a>Создание Фонеаусентикатионмесод

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление нового [метода проверки подлинности телефона](../resources/phoneauthenticationmethod.md). У пользователя может быть только один телефон каждого типа, записанный в свойстве **фонетипе** . Это означает, что, например, `mobile` при добавлении телефона в пользователя с уже существующим `mobile` телефоном произойдет ошибка. Кроме того, перед добавлением телефона у пользователя всегда должен быть `mobile` Телефон `alternateMobile` .

Добавление телефонного номера делает его доступным для использования в Azure Multi-Factor Authentication (MFA) и самостоятельном сбросе пароля (SSPR), если он включен.

Кроме того, если для пользователя включена политика для входа в SMS и `mobile` добавляется номер, система попытается зарегистрировать номер для использования в этой системе.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения, действующие на себя (по крайней мере для самых привилегированных) | Разрешения, действующие на других (по крайней мере для самых привилегированных)|
|:---------------------------------------|:-------------------------|:-----------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. | Усераусентикатионмесод. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. | Не поддерживается. |
| Для приложений                            | Не поддерживается. | Не поддерживается. |

Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id}/authentication/phoneMethods
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в формате JSON. Формат JSON должен включать `phoneNumber` и `phoneType` , но не `smsSignInState` (доступен только для чтения).

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|phoneNumber|String|Номер телефона для текста или вызов для проверки подлинности. Номера телефонов используют формат "+ \<country code\> \<number\> x \<extension\> " с необязательным расширением. Например, допустимые + 1 5555551234 или + 1 5555551234x123. При создании или обновлении числа отклоняются, если они не совпадают с требуемым форматом.|
|фонетипе|String|Возможные значения: `mobile` , `alternateMobile` и `office` .|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
