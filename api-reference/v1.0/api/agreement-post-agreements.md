---
title: Создание соглашения
description: Создание нового объекта соглашения.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: f978b9599b2427dc06173636cd19ead373f8c56d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017046"
---
# <a name="create-agreement"></a>Создание соглашения

Пространство имен: microsoft.graph

Создание нового [объекта соглашения.](../resources/agreement.md)
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Agreement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [соглашения.](../resources/agreement.md)

В следующей таблице показаны свойства, необходимые при создании соглашения.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображение имени соглашения.|
|isViewingBeforeAcceptanceRequired|Логический|Указывает, должен ли пользователь расширять и просматривать соглашение перед принятием.|
|fileName|String|Имя файла соглашения (например, TOU.pdf).|
|isDefault|Boolean|Указывает, является ли это файл соглашения по умолчанию, если язык соответствует предпочтениям клиента. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию.|
|language|String|Язык файла соглашения в формате languagecode2-country/regioncode2. languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1. country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).|
|data|В двоичном формате|Данные, которые представляют условия использования документа PDF.|

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201, Created` объект соглашения в тексте ответа. [](../resources/agreement.md)

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В органе запроса поставляем представление JSON объекта [соглашения.](../resources/agreement.md)


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


