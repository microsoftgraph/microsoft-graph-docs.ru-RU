---
title: Обновление organizationalBrandingLocalization
description: Обновление свойств объекта organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8fa2a1eb9f22c1055bb99666f4845a3a8505ffe0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443314"
---
# <a name="update-organizationalbrandinglocalization"></a>Обновление organizationalBrandingLocalization
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) для определенной локализации.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

С помощью метода PUT обновляются только типы данных Stream, включая **backgroundLogo** и **backgroundImage**. Чтобы обновить строковые типы данных, включая **signInPageText** и **usernameHintText**, используйте метод PATCH. Нельзя обновить типы потоков с помощью других типов данных в том же запросе.

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
PUT /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}/{backgroundImage | bannerLogo | squareLogo}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, отображаемый вместо фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в шестнадцатеричном формате, например белый.`#FFFFFF` |
| Backgroundimage | Stream | Изображение, отображаемое в качестве фона страницы входа. Допустимые типы: PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Изображение меньшего размера уменьшит требования к пропускной способности и ускорит загрузку страницы. |
| bannerLogo | Stream | Баннер с логотипом компании, который отображается на странице входа. Допустимые типы: PNG или JPEG размером не более 36 × 245 пикселей. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа. |
| customAccountResetCredentialsUrl | String | Настраиваемый URL-адрес для сброса учетных данных учетной записи. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128 символов. |
| customCannotAccessYourAccountText | String | Строка для замены значения по умолчанию "Не удается получить доступ к учетной записи?" Текст гиперссылки для самостоятельного сброса пароля (SSPR) на странице входа. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customForgotMyPasswordText | String | Строка для замены текста гиперссылки "Забыли пароль" по умолчанию в форме входа. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customPrivacyAndCookiesText | String | Строка для замены текста гиперссылки "Конфиденциальность и файлы cookie" по умолчанию в нижнем колонтитуле. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customPrivacyAndCookiesUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Конфиденциальность и файлы cookie" в нижнем колонтитуле. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128 символов. |
| customTermsOfUseText | String | Строка для замены текста гиперссылки "Условия использования" по умолчанию в нижнем колонтитуле. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customTermsOfUseUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Условия использования" в нижнем колонтитуле. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128character. |
| Значок | Stream | Пользовательский значок (favicon) для замены значка продукта Майкрософт по умолчанию в Azure AD клиенте. |
| headerBackgroundColor | String | Цвет RGB, применяемый для настройки цвета заголовка. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | Представляет различные тексты, которые могут быть скрыты на странице входа для клиента. Все свойства можно обновить. |
| signInPageText | String | Текст, отображаемый в нижней части поля входа. Используйте его для передачи дополнительных сведений, таких как номер телефона в службу технической поддержки или юридическое заявление. Этот текст должен быть в формате Юникода и не превышать 1024 символа. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 при первом включении компьютера (OOBE) и когда Windows Autopilot включен для развертывания. Допустимые типы: PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа.|
| usernameHintText | String | Строка, отображаемая в качестве подсказки в текстовом поле имени пользователя на экране входа. Этот текст должен быть Юникодом без ссылок или кода и не может превышать 64 символа. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-setting-bannerlogo-for-the-fr-fr-localization-using-put"></a>Пример 1. Настройка **bannerLogo** для локализации fr-FR с помощью PUT

Следующий запрос обновляет логотип баннера для локализации fr-FR.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-the-backgroundcolor-and-signinpagetext-for-the-fr-fr-localization-using-patch"></a>Пример 2. Обновление backgroundColor и signInPageText для локализации fr-FR с помощью PATCH

Следующий запрос обновляет логотип баннера для локализации `fr-FR` .

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization6"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "Welcome to Contoso France"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization6-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization6-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-a-default-branding-value-with-a-blank-string"></a>Пример 3. Переопределение значения фирменной символики по умолчанию пустой строкой

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization7"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "signInPageText": "Welcome to Contoso France.",
    "usernameHintText":" "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization7-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization7-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

После запроса **usernameHintText** `fr-FR` для локализации будет пустым, а не наследовать значение от объекта фирменной символики по умолчанию.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
