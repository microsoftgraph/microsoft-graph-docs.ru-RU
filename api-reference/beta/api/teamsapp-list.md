---
title: Список опубликованных приложений из каталога приложений Microsoft Teams
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a27a7b63248ddb94e4ea819300f325e04a02c9f
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636520"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Список опубликованных приложений из каталога приложений Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.
Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента). Чтобы получить доступ к приложениям только из каталога приложений вашей организации, `Organization` укажите в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions_reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | AppCatalog.ReadWrite.All            |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                       |
| Для приложений                            | Не поддерживается                       |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Нет.

> **Примечание:** Можно выполнить фильтрацию по любому полю объекта [теамскаталогапп](../resources/teamsapp.md) для сокращения списка результатов. Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [теамскаталогапп](../resources/teamsapp.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-applications"></a>Пример 1: List All Applications

В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

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

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>Отклик

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

