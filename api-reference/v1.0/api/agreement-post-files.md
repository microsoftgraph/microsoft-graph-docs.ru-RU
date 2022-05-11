---
title: Создание agreementFileLocalization
description: Создайте файл локализованного соглашения.
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 71f5568c369e1642ac3725fcc34612de5a8c1d30
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315106"
---
# <a name="create-agreementfilelocalization"></a>Создание agreementFileLocalization
Пространство имен: microsoft.graph

Создайте файл локализованного соглашения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Agreement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /agreements/{agreementsId}/files
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [agreementFileLocalization](../resources/agreementfilelocalization.md) в формате JSON.

При создании **agreementFileLocalization** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованное отображаемое имя файла политики соглашения. Локализованное отображаемое имя отображается пользователям, просматривая соглашение.|
|fileData|[agreementFileData](../resources/agreementfiledata.md)|Данные, которые представляют условия использования PDF-документа.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). |
|isDefault|Boolean|Если ни один из языков не соответствует предпочтениям клиента, указывает, является ли это файл соглашения по умолчанию. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как файл по умолчанию. Только для чтения.|
|isMajorVersion|Boolean|Указывает, является ли файл соглашения основным обновлением версии. Обновления основных версий недействительны для принятия условий соглашения на соответствующем языке.|
|language|String|Язык файла соглашения в формате languagecode2-country/regioncode2. Languagecode2 — это двухбуквенный код в нижнем регистре, производный от ISO 639-1, а "country/regioncode2" является производным от ISO 3166 и обычно состоит из двух прописных букв или языкового тега BCP-47. Например, английский (США) — `en-US`.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [agreementFileLocalization](../resources/agreementfilelocalization.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_agreementfilelocalization_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/files
Content-Type: application/json

{
    "fileName": "Contoso ToU for guest users (French)",
    "language": "fr-FR",
    "isDefault": false,
    "isMajorVersion": false,
    "displayName": "Contoso ToU for guest users (French)",
    "fileData": {
        "data": "base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data"
    }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/termsOfUse/agreements('94410bbf-3d3e-4683-8149-f034e55c39dd')/files/$entity",
    "id": "90d1723c-52c1-40e3-a51a-da99a82c0327",
    "fileName": "Contoso ToU for guest users (French)",
    "displayName": "Contoso ToU for guest users (French)",
    "language": "fr-FR",
    "isDefault": false,
    "isMajorVersion": false,
    "createdDateTime": "2022-03-04T14:38:22.8292386Z",
    "fileData": {
        "data": "base64JVBERi0xLjUKJb/"
    }
}
```
