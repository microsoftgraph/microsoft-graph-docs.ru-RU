---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa995b4b545eb2f9f7ea42d9fd9d8744a0a656cb
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843179"
---
# <a name="list-teamsapp"></a>Список teamsApp

Пространство имен: microsoft.graph

Список [приложений](../resources/teamsapp.md) , опубликованных в каталоге приложений Microsoft Teams. Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента). Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

> **Примечание:** Только глобальные администраторы могут вызывать этот API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                       |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.

При использовании `$expand=AppDefinitions` будут возвращены дополнительные сведения о состоянии приложения. 

> **Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов. Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-applications-in-your-tenant"></a>Пример 1: список всех приложений в клиенте

В следующем примере перечисляются все приложения, характерные для вашего клиента.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом

В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
