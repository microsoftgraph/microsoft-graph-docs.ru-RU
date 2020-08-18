---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 613011ce44b05b1743a8d297fc63450d4eed7dee
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790744"
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

> **Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов. Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

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

#### <a name="response"></a>Ответ

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

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

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
