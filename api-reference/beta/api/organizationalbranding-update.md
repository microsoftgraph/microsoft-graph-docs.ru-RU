---
title: Обновление organizationalBranding
description: Обновление свойств объекта organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 073422bb2d6d831c8640de781aa4b6093b5025ba
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804488"
---
# <a name="update-organizationalbranding"></a>Обновление organizationalBranding
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта брендинга по умолчанию, заданного [ресурсом organizationalBranding](../resources/organizationalbranding.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|
|Принять-Язык|Допустимый локал ISO 639-1. Обязательно.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который отображается на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый .`#FFFFFF` |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
| customAccountResetCredentialsUrl | String | Настраиваемый URL-адрес для сброса учетных данных учетных записей. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. |
| customCannotAccessYourAccountText | String | Строка для замены по умолчанию "Не может получить доступ к учетной записи?" текст гиперссылки самообслуживляемого сброса пароля (SSPR) на странице вход. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customForgotMyPasswordText | String | Строка для замены текста гиперссылки по умолчанию "Забыл пароль" в форме входного знака. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customPrivacyAndCookiesText | String | Строка для замены текста гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customPrivacyAndCookiesUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. |
| customTermsOfUseText | String | Строка для замены текста гиперссылки по умолчанию "Термины использования" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customTermsOfUseUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Условия использования" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128characters. |
| favicon | Stream | Настраиваемый значок (favicon) для замены фавикона продукта Microsoft по умолчанию на клиенте Azure AD. |
| headerBackgroundColor | String | Цвет RGB, который необходимо применить для настройки цвета загона. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | Представляет различные тексты, которые можно скрыть на странице входа для клиента. Все свойства можно обновить. |
| signInPageText | String | Текст, который отображается в нижней части окна для регистрации. Используйте это для получения дополнительных сведений, например номера телефона в службе поддержки или юридического заявления. Этот текст должен быть в формате Unicode и не превышать 1024 символов. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Допустимые типы PNG или JPEG не более 240 x 240 пикселей и не более 10 КБ в размере. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
| usernameHintText | String | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране регистрации. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-the-default-branding"></a>Пример 1. Обновление брендинга по умолчанию

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_1"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Accept-Language: 0

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocaliation-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocaliation-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocaliation-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocaliation-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocaliation-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocaliation-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-the-default-branding"></a>Пример 2. Обновление bannerLogo для брендинга по умолчанию

Следующий запрос обновляет логотип баннера для фирменого знака по умолчанию.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.



<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_2"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
