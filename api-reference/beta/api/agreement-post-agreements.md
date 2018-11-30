---
title: Создание соглашения
description: Создайте новый объект соглашения.
ms.openlocfilehash: bfcab53b4233d133309c99a4825e184a42670458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076038"
---
# <a name="create-agreement"></a>Создание соглашения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Создайте новый объект [соглашения](../resources/agreement.md) .
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
POST /agreements
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный атрибут. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.

В приведенной ниже таблице показаны обязательные свойства при создании пользователя.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображаемое имя соглашения.|
|isViewingBeforeAcceptanceRequired|Логический|Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.|
|файлы и имя файла|String|Имя файла соглашения (например, TOU.pdf).|
|файлы/isDefault|Логический|Указывает, является ли файл соглашения по умолчанию Если ни одна из языка и региональных параметров соответствует предпочтений клиента. Если ни одна из файл помечен как по умолчанию, первый будет рассматриваться как по умолчанию.|
|файлы/языка|String|Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2. languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1. Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US).|
|файлы/fileData/БД|Двоичный|Данные, представляющие условия использования PDF-документа.|

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201, Created` объект [соглашение](../resources/agreement.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
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

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
