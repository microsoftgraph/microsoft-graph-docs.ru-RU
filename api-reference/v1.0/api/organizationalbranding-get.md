---
title: Get organizationalBranding
description: Ознакомьтесь с свойствами и отношениями объекта organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26471f66b85f4fab78c9ac9c46de4f9a3513498c
ms.sourcegitcommit: 7ce66321abb6a2cdca8685d3ce0a004c376ae33b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59778042"
---
# <a name="get-organizationalbranding"></a>Get organizationalBranding
Пространство имен: microsoft.graph

Извлечение объекта организационного брендинга по умолчанию, если заготвка **Accept-Language** не указана. Если объект организационного брендинга не создан, этот метод возвращает `404 Not Found` ошибку.

Если **заготвка Accept-Language** задана, этот метод извлекает брендинг для указанного локального языка.

Этот метод извлекает только свойства, не веские, например имя **пользователяHintText** и **signInPageText**. Чтобы получить потоковые типы брендинга по умолчанию, например **bannerLogo** и **backgroundImage,** используйте [метод GET organizationalBrandingLocalization.](organizationalbrandinglocalization-get.md) ID **для** локализации по умолчанию может быть `0` или `default` .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User.Read, Organization.Read.All, User.ReadBasic.All, User.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/branding
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает только параметр `$select` запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Принять-Язык|Допустимый локал ISO 639-1. Необязательное свойство.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект organizationalBranding](../resources/organizationalbranding.md) в тексте отклика. Если нет объекта брендинга по умолчанию, этот метод возвращает `404 Not Found` код ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-default-branding"></a>Пример 1. Получить брендинг по умолчанию

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#branding",
    "@odata.id": "https://graph.microsoft.com/v2/99b24e1b-abec-4598-9d63-a2baf0a3cea1/directoryObjects/$/Microsoft.DirectoryServices.Organization('99b24e1b-abec-4598-9d63-a2baf0a3cea1')/branding/0",
    "id": "0",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/illustration?ts=637535563816027796",
    "bannerLogoRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/bannerlogo?ts=637535563824629275",
    "cdnList": [
        "secure.aadcdn.microsoftonline-p.com",
        "aadcdn.msftauthimages.net",
        "aadcdn.msauthimages.net"
    ],
    "signInPageText": "Contoso",
    "squareLogoRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/tilelogo?ts=637535563832888580",
    "usernameHintText": ""
}
```


### <a name="example-2-get-organizational-branding-when-no-branding-is-configured"></a>Пример 2. Получить организационный брендинг, если брендинг не настроен

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_Error"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 404 Not Found
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a>Пример 3. Получить организационный брендинг для французского языка

В следующем примере используется заглавный заготок **Accept-Language,** который указывает для получения брендинг локализации.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_locale"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr-FR
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#branding",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/$/Microsoft.DirectoryServices.Organization('84841066-274d-4ec0-a5c1-276be684bdd3')/branding/fr",
    "id": "fr",
    "backgroundColor": "#FFFF33",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": " "
}
```

### <a name="example-4-get-the-bannerlogo-for-the-default-locale"></a>Пример 4. Получить bannerLogo для локального значения по умолчанию

В следующем примере **возвращается объект bannerLogo** для локального значения по умолчанию. Вы можете указать **id** как `default` или в `0` URL-адресе запроса. Если объект не установлен, запрос возвращает пустой ответ.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_organizationalbranding_defaultlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: image/*

<Image>
```

### <a name="example-5-get-the-bannerlogo-for-the-fr-fr-locale"></a>Пример 5. Получить bannerLogo для fr-FR-locale

В следующем примере возвращается **объект bannerLogo** для локального `fr-FR` объекта, чей bannerLogo не установлен.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_frlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK

{}
```