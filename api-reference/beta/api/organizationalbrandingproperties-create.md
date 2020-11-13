---
title: Создание Организатионалбрандингпропертиес
description: Создание фирменной символики Организации.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efb10cd5669022dda2afd385ea013ae110a97ea0
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031998"
---
# <a name="create-organizationalbrandingproperties"></a>Создание Организатионалбрандингпропертиес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) . При этом создается фирменная символика по умолчанию и, при необходимости, локализованная фирменная символика. Фирменная символика по умолчанию загружается, когда локализованный набор фирменного стиля не настроен для языка браузера пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Фирменная символика создается для Организации, если она еще не существует, с помощью функции "вставить" или "исправить".

Если фирменная символика уже настроена, при РАЗМЕЩЕНии будут перезаписаны все существующие значения независимо от того, что находится в теле запроса. PATCH будет оверите только значения, включенные в текст запроса, оставляя значения, не включенные в неизмененное.

Свойство **ID** игнорируется на странице PUT/patch для одноэлементного экземпляра/брандинг. Если язык содержимого не указан, создается фирменная символика по умолчанию, соответствующая **идентификатору** `und` . Если указан язык содержимого, для этого языкового стандарта создается фирменная символика.
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Content — Language  | Языковой стандарт. Необязательный параметр.  |

## <a name="request-body"></a>Текст запроса

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|баккграундколор|Строка|Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации. Укажите в шестнадцатеричном формате (например, белый #FFFFFF).|
|Изображение|Stream|Изображение, отображаемое в качестве фона страницы входа. файлы PNG или jpg не больше 1920x1080 и меньше 300kb. Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.|
|баннерлого|Stream|На странице входа отображается плакатная эмблема компании. файлы PNG или jpg не больше 36x245px. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|сигнинпажетекст|Строка|Текст, который отображается в нижней части поля входа. Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет. Этот текст должен быть Юникодом и не превышать 1024 символов.|
|скуарелого|Stream|Квадратная версия логотипа компании. Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows. файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|усернамехинттекст|Строка|Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа. Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и созданный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.

## <a name="examples"></a>Примеры

В следующем примере показано, как создать фирменную символику и локализацию по умолчанию для en/US.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

В этом случае задается объект фирменной символики по умолчанию. Локализованная фирменная символика для en-US также устанавливается из-за того, что в заголовке используется язык контента, даже если в ответе не возвращается набор фирменной символики en-US. Обратите внимание на то, что язык контента в запросе является необязательным, и если он отсутствует, будет задана фирменная символика по умолчанию.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
