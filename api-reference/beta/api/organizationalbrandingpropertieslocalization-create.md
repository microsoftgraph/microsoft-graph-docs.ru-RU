---
title: Создание локализованных организационных свойствBrandingProperties
description: Создание фирменого бренда организации для определенного локального.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7e3108da9ed5251b9f041dc710c16bff674c8a01
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447827"
---
# <a name="create-localized-organizationalbrandingproperties"></a>Создание локализованных организационных свойствBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) для определенного локального объекта.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

POST для создания новой локализации. Указанный в теле id — это локализовка для локализации. Если не указан id, то в качестве id используется значение загона Content-Language, если указано. Если не указаны id и не указаны заглавные материалы на языке контента, возвращается ошибка.
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Content-Language  | Locale. Необязательный параметр.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|backgroundColor|String|Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal (например, белый #FFFFFF).|
|backgroundImage|Stream|Изображение, которое отображается в качестве фона знака на странице. .png или .jpg не больше 1920x1080 и меньше 300kb. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.|
|bannerLogo|Stream|На странице входного знака отображается баннерная версия логотипа вашей компании. .png или .jpg не больше 36x245px. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
|signInPageText|String|Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов.|
|squareLogo|Stream|Квадратная версия логотипа вашей компании. Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания. .png или .jpg размером не более 240x240px и размером не более 10 кб. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
|usernameHintText|String|Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака. Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.|
|id|String|Locale для создания брендинга для|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и созданный `201 CREATED` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.

## <a name="examples"></a>Примеры

В следующем примере создается локализация бренда для французского языка (fr).

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
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

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
**MediaEditLink** указывает, где записано локализованные носители. MediaReadLink является null, так как для локализации не установлено мультимедиа.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
