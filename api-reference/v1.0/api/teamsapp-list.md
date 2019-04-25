---
title: Список опубликованных приложений из каталога приложений Microsoft Teams
description: 'ПереЧисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 884fd932acddb1352c48e82302a6c345fadf90b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521791"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Список опубликованных приложений из каталога приложений Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ПереЧисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.
Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента). Чтобы получить доступ к приложениям только из каталога приложений вашей организации, `Organization` укажите в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).

> **Примечание:** Только глобальные администраторы могут вызывать этот API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.ReadWrite.All            |
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

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
