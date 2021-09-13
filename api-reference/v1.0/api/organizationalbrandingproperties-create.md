---
title: Создание organizationalBrandingProperties
description: Создание фирменого бренда организации.
ms.localizationpriority: medium
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 50a4253b9ae53df765bd65708284b7a2c5d90cb8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59079221"
---
# <a name="create-organizationalbrandingproperties"></a>Создание organizationalBrandingProperties

Создание [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md) Это создает брендинг по умолчанию и необязательно локализованный брендинг. Брендинг по умолчанию загружается, когда локализованный набор брендинга не настроен на язык браузера пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Брендинг создается для организации, если она еще не существует, с помощью PUT или PATCH.

Если брендинг уже настроен, PUT переописает все существующие значения независимо от того, что находится в теле запроса. PATCH только переописывает значения, включенные в тело запроса, в результате чего значения не остаются неизменными.

Свойство `id` игнорируется в PUT/PATCH в синглтоне /branding. Если **язык контента** не указан, создается брендинг по умолчанию, соответствующий `id` одному из `und` . Если **задан язык** контента, для этого языка создается брендинг.
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{tenant id}/branding
PATCH /organization/{tenant id}/branding
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Content-Language  | Locale. Необязательно.  |

## <a name="request-body"></a>Текст запроса

В орган запроса включаем представление JSON объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md) В следующей таблице перечислены необходимые свойства.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|backgroundColor|String|Цвет, который отображается на месте фонового изображения в подключениях с низкой пропускной способностью. Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal (например, белый #FFFFFF).|
|backgroundImage|Stream|Изображение, которое отображается в качестве фона страницы регистрации. Изображение — это .png или .jpg размером не более 1920x1080 и меньше 300 кб. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.|
|bannerLogo|Stream|Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Баннер — это .png или .jpg размером не более 36x245px. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
|signInPageText|Строка|Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов.|
|squareLogo|Stream|Квадратная версия логотипа вашей компании. Это отображается в Windows 10(OOBE) и когда Windows автопилот включен для развертывания. Логотип представляет .png или .jpg размером не более 240x240px и размером не более 10 кб. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
|usernameHintText|Строка|Подсказка в текстовом ящике имени пользователя на экране входной записи. Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и созданный `201 Created` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.

## <a name="examples"></a>Примеры

В следующем примере создается брендинг по умолчанию и локализация **контент-языка.** `en-US`

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_1"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

В этом случае заданной является объект брендинга по умолчанию. Локализованная торговая марка также устанавливается из-за загона Content-Language, даже несмотря на то, что набор брендинга не возвращается `en-US` в  `en-US` ответе. **Заготвка Content-Language** в запросе необязательна, и если ее нет, она задает только брендинг по умолчанию.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
