---
title: Создание локализованных Организатионалбрандингпропертиес
description: Создание фирменной символики Организации для определенного языкового стандарта.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c293085887eb0e8c2d49c4e01c567dbeea32699
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524432"
---
# <a name="create-localized-organizationalbrandingproperties"></a>Создание локализованных Организатионалбрандингпропертиес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) для определенного языкового стандарта.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Разместите в фирменной символике/локализации, чтобы создать новую локализацию. Идентификатор, указанный в теле, — это языковой стандарт локализации. Если идентификатор не указан, то в качестве идентификатора используется значение заголовка Content-Language, если оно указано. Если заголовок ID и Content-Language не указаны, возвращается ошибка.
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
| Content — Language  | Языковой стандарт. Необязательный параметр.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|баккграундколор|String|Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации. Укажите в шестнадцатеричном формате (например, белый #FFFFFF).|
|Изображение|Stream|Изображение, отображаемое в качестве фона страницы входа. файлы PNG или jpg не больше 1920x1080 и меньше 300kb. Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.|
|баннерлого|Stream|На странице входа отображается плакатная эмблема компании. файлы PNG или jpg не больше 36x245px. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|сигнинпажетекст|String|Текст, который отображается в нижней части поля входа. Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет. Этот текст должен быть Юникодом и не превышать 1024 символов.|
|скуарелого|Stream|Квадратная версия логотипа компании. Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows. файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|усернамехинттекст|String|Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа. Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.|
|id|String|Языковой стандарт для создания фирменной символики для|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 CREATED` код отклика и созданный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере создается локализация фирменного стиля для французского языка (fr).

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

Ниже приведен пример ответа.

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
**Медиаедитлинк** указывает, где записывается локализованный носитель. Медиареадлинк имеет значение null, так как для локализации не задан носитель.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
