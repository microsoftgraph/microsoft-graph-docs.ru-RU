---
title: Обновление organizationalBranding
description: Обновление свойств объекта organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6dbcccc8fb457d8a34dc62b366c46e1bf845f4a6
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971177"
---
# <a name="update-organizationalbranding"></a>Обновление organizationalBranding
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойства объекта фирменной символики по умолчанию, указанного [ресурсом organizationalBranding](../resources/organizationalbranding.md) .

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
|Принять-Язык|Допустимый языковой стандарт ISO 639-1 или `0` языковой стандарт по умолчанию. Обязательный элемент.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | Строка | Цвет, отображаемый вместо фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в шестнадцатеричном формате, например белый.`#FFFFFF` |
| Backgroundimage | Stream | Изображение, отображаемое в качестве фона страницы входа. Допустимые типы: PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Изображение меньшего размера уменьшит требования к пропускной способности и ускорит загрузку страницы. |
| bannerLogo | Stream | Баннер с логотипом компании, который отображается на странице входа. Допустимые типы: PNG или JPEG размером не более 36 × 245 пикселей. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа. |
| customAccountResetCredentialsUrl | Строка | Настраиваемый URL-адрес для сброса учетных данных учетной записи. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128 символов. |
| customCannotAccessYourAccountText | Строка | Строка для замены значения по умолчанию "Не удается получить доступ к учетной записи?" Текст гиперссылки для самостоятельного сброса пароля (SSPR) на странице входа. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customForgotMyPasswordText | Строка | Строка для замены текста гиперссылки "Забыли пароль" по умолчанию в форме входа. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customPrivacyAndCookiesText | Строка | Строка для замены текста гиперссылки "Конфиденциальность и файлы cookie" по умолчанию в нижнем колонтитуле. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customPrivacyAndCookiesUrl | Строка | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Конфиденциальность и файлы cookie" в нижнем колонтитуле. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128 символов. |
| customTermsOfUseText | Строка | Строка для замены текста гиперссылки "Условия использования" по умолчанию в нижнем колонтитуле. Этот текст должен быть в формате Юникода и не превышать 256 символов. |
| customTermsOfUseUrl | Строка | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Условия использования" в нижнем колонтитуле. Этот URL-адрес должен быть в формате ASCII или символы, отличные от ASCII, должны быть закодированными URL-адресами и не превышать 128character. |
| Значок | Stream | Пользовательский значок (favicon) для замены значка продукта Майкрософт по умолчанию в клиенте Azure AD. |
| headerBackgroundColor | Строка | Цвет RGB, применяемый для настройки цвета заголовка. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | Представляет различные тексты, которые могут быть скрыты на странице входа для клиента. Все свойства можно обновить. |
| signInPageText | Строка | Текст, отображаемый в нижней части поля входа. Используйте его для передачи дополнительных сведений, таких как номер телефона в службу технической поддержки или юридическое заявление. Этот текст должен быть в формате Юникода и не превышать 1024 символа. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается в windows 10 в режиме запуска при первом включении при первом включении, и когда Windows Autopilot включен для развертывания. Допустимые типы: PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа.|
| usernameHintText | Строка | Строка, отображаемая в качестве подсказки в текстовом поле имени пользователя на экране входа. Этот текст должен быть Юникодом без ссылок или кода и не может превышать 64 символа. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-the-default-branding"></a>Пример 1. Обновление фирменной символики по умолчанию

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

### <a name="example-2-update-bannerlogo-for-the-default-branding"></a>Пример 2. Обновление bannerLogo для фирменной символики по умолчанию

Следующий запрос обновляет логотип баннера для фирменной символики по умолчанию.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.




# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_2"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocaliation-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocaliation-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
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
