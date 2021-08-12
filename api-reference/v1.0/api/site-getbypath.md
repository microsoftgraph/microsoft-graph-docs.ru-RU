---
author: JeremyKelley
ms.date: 09/10/2017
title: Получить SharePoint по пути
localization_priority: Normal
ms.prod: sharepoint
description: Получение свойств и отношений ресурса site.
doc_type: apiPageType
ms.openlocfilehash: 33f1d31188e679ffdc271604f016fe5849a9075bad9add8929ea6bd872bc4b50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155297"
---
# <a name="get-a-site-resource-by-path"></a>Получение ресурса site по его пути

Пространство имен: microsoft.graph

Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.

[site]: ../resources/site.md

Помимо получения ресурса [site по его идентификатору](site-get.md) вы можете получить ресурс site, используя URL-адрес, относительный для сервера.

* Имя узла семейства веб-сайтов (contoso.sharepoint.com).
* Путь к сайту, относительный для имени узла сервера.

Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.

* `/sites/root`. Корневой сайт клиента.
* `/groups/{group-id}/sites/root`. Сайт группы для ресурса group.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы получить доступ к корневому сайту SharePoint с использованием относительного пути, выполните указанные ниже действия.

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a>Отклик

Этот метод возвращает ресурс [site][] для сайта, для ссылки на который используется уникальный идентификатор.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": "Sites/Get by path"
} -->

