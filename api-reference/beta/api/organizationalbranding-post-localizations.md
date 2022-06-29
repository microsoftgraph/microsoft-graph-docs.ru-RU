---
title: Создание organizationalBrandingLocalization
description: Создайте объект organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 027cbe6d197e2482d41605027bc565baf73eb16a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443298"
---
# <a name="create-organizationalbrandinglocalization"></a>Создание organizationalBrandingLocalization
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [organizationalBrandingLocalization](../resources/organizationalBrandingLocalization.md) . При этом создается локализованная фирменная символика, а в то же время — фирменная символика по умолчанию, если она не существует.

Фирменная символика по умолчанию создается только один раз. Он загружается, если локализованная фирменная символика не настроена для языка браузера пользователя. Сведения о том, как получить фирменную символику по умолчанию, см. [в разделе "Получение фирменной символики"](organizationalbranding-get.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
Этот запрос создает новую фирменную символику локализации и фирменную символику по умолчанию, если она еще не существует. 
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/branding/localizations
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В следующей таблице показаны свойства, необходимые при создании объекта [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Идентификатор, представляющий языковой стандарт, указанный с использованием имен языков и региональных параметров. Имена языков и региональных параметров соответствуют стандарту RFC 1766 в формате languagecode2-country/regioncode2, где "languagecode2" — это двухбуквенный двухбуквенный код в нижнем регистре, производный от ISO 639-1, а "country/regioncode2" — это двухбуквенный код в верхнем регистре, производный от ISO 3166. Например, английский (США) — `en-US`. Вы не можете создать фирменную символику по умолчанию, заключив значение **идентификатора** в строковые типы или `0` `default`.  <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменной символики для одного языкового стандарта в настоящее время не поддерживаются. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) в тексте отклика.

## <a name="examples"></a>Примеры

В следующем примере создается локализация фирменной символики для локализации на французском языке (`fr-FR`). Все неуказанные свойства типа String наследуются от значения в объекте фирменной символики по умолчанию. Например, если signInPageText `null`в объекте фирменной символики по умолчанию имеет значение signInPageText `fr-FR` для фирменной символики, созданной в этом запросе, также будет иметь значение `null`. Чтобы переопределить значение `null` без текста, используйте строку, содержащую только пробелы.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr-FR",
    "signInPageText": " "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-organizationalbrandinglocalization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-organizationalbrandinglocalization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-organizationalbrandinglocalization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-organizationalbrandinglocalization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-organizationalbrandinglocalization-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-organizationalbrandinglocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')/branding/localizations/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/directoryObjects/$/Microsoft.DirectoryServices.Organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')//localizations/fr-FR",
    "id": "fr-FR",
    "backgroundColor": " ",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": " "
}
```
