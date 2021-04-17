---
title: Get teamworkHostedContent
description: Извлечение содержимого в teamsAppIcon.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b5fde96ffaad34360603751398473357d82e1fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882701"
---
# <a name="get-teamworkhostedcontent"></a>Get teamworkHostedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Извлечение содержимого в](../resources/teamworkhostedcontent.md) [значке приложения.](../resources/teamsappicon.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-for-app-icon-in-app-catalog"></a>Разрешения на значок приложения в каталоге приложений
| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                   |
| Для приложений                            | Не поддерживается.                                                   |

## <a name="http-request"></a>HTTP-запрос

**Создание содержимого в значке приложения в каталоге приложений**

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта операция поддерживает `$select` [параметры запроса OData](/graph/query-parameter) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок           | Значение                      |
| :--------------- | :------------------------- |
| Авторизация    | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект teamworkHostedContent](../resources/teamworkhostedcontent.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a>Пример 1. Получить в каталоге биты содержимого значка цвета приложения Teams

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```


#### <a name="response"></a>Отклик

Ниже показан пример отклика.

> **Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a>Пример 2. Получить в каталоге биты содержимого иконки контура приложения Teams

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

> **Примечание:** Запросы на необработанные значения не поддерживают параметры [запроса OData](/graph/query-parameters) для настройки ответа.

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```

#### <a name="response"></a>Отклик

Ответ содержит bytes для размещенного контента в теле. `content-type` Заглавный заглавник указывает тип содержимого, на который установлено.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a>См. также

- [Получить значки приложения Teams](teamsappicon-get.md)
- [Список приложений в каталоге](appcatalogs-list-teamsapps.md)
