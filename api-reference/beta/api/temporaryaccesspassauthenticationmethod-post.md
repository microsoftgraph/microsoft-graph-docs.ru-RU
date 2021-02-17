---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d048d843c0a93dc779a0966d6a27d337251fc974
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272687"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a>Создание temporaryAccessPassAuthenticationMethod
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [временный объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя. У пользователя может быть только один временный проход доступа. Пароль можно использовать между началом и временем окончания временного прохода доступа. Если пользователю требуется новый временный проход доступа:
* Несмотря на то что текущий временный проход доступа действителен, администратору необходимо удалить существующий временный проход доступа и создать новый проход для пользователя. При удалении действительного временного прохода сеансы пользователя будут отоскины. 
* По истечении срока действия временного доступа новый временный проход доступа переопределяет текущий временный проход доступа и не отменяет сеансы пользователя.


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Разрешения, действующие на себя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="permissions-acting-on-other-users"></a>Разрешения, действующие с другими пользователями

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|:-----------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | UserAuthenticationMethod.ReadWrite.All |

Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в JSON.

В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временного объектаAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)

|Свойство|Тип|Описание|Обязательный| 
|:---|:---|:---|:---|
|startDateTime|DateTimeOffset|Дата и время, когда временныйaccessPass становится доступным для использования, если не задав временный проход доступа, доступен для использования во время создания.| Нет|
|lifetimeInMinutes|Int32|Время существования temporaryAccessPass в минутах, начиная с момента создания или в startDateTime, если установлено. Минимум 10, максимум 43200 (эквивалентно 30 дням).| Нет|
|isUsableOnce|Boolean|Определяет, ограничен ли проход одновейным использованием. Если имеет значение True, то проход можно использовать один раз, если задав значение False, этот проход можно использовать несколько раз в течение жизненного времени temporaryAccessPass. A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.|  Нет|



## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код отклика и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
  "lifetimeInMinutes": 60,
  "isUsableOnce": false
}
```

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```