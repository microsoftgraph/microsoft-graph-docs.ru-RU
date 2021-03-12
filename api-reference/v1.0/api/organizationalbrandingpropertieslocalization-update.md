---
title: Обновление локализованных свойств организационногобрендинга
description: Обновление свойств объекта организационныхбрандингов для определенной локализации.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0c38656b71c2fdc5b3832a106effecfe9970c811
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722634"
---
# <a name="update-localized-organizationalbrandingproperties"></a>Обновление локализованных свойств организационногобрендинга

Обновление свойств объекта [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) для определенной локализации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Content-Language  | Locale. Необязательное свойство.  |

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
|id|String|Locale для обновления брендинга для|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 OK`.

## <a name="examples"></a>Примеры

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a>Пример 1. Настройка **bannerLogo** для локализации fr с помощью PUT

Следующий запрос обновляет логотип баннера для `fr` локализации. С помощью PUT, если локализация fr не существует, возвращается `404 not found` ошибка. Если в полезной нагрузке содержится свойство или заглавное свойство Content-Language и они не совпадают с `id` **URL-адресом,** возвращается `id` `Bad Request` ошибка.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a>Пример 2. Обновление **bannerLogo** для локализации fr с помощью PATCH

Следующий запрос обновляет логотип баннера для локализации fr.  С помощью PATCH, если указанная локализация еще не существует, она создается и свойство записано на него.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-override-default-branding-value-with-a-blank-string"></a>Пример 3. Переопределение значения брендинга по умолчанию с пустой строкой

Если значение свойства в локализации является null, это значение будет унаследовано от фирменного бренда по умолчанию. Чтобы этого не произошло, установите пустую строку или строку, содержащую только белое пространство в локализованной фирме.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

После этого запроса имя пользователяHintText для локализации fr будет пустым, а не наследуется значение от брендинга по умолчанию.

### <a name="example-4-replace-french-localization-with-put"></a>Пример 4. Замена французской локализации на PUT

Чтобы сделать обновление по локализации с помощью PUT, мы должны добавить все свойства в теле вместе с свойством, которое необходимо обновить по мере замены существующего объекта на новый. Другие свойства, которые не находятся в теле полезной нагрузки PUT, будут настроены на NULL. В приведенном ниже примере сохраняется только свойство backgroundColor и обновляется signInPageText, в то время как для других установлено null.
Если указанная локализация еще не существует, ВСТАВЬТЕ в URL-адрес с указанием, что локализация создает ее.
Если в полезной нагрузке содержится свойство id или заглавное свойство Content-Language, и они не совпадают с id в URL-адресе, мы бросаем плохой запрос.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
