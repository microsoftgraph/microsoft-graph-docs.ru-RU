---
author: JeremyKelley
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
ms.date: 09/10/2017
title: Получение предыдущей версии записи списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 81fdde8bf750839a278da9857281d59886407657
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957942"
---
# <a name="list-versions-of-a-listitem"></a><span data-ttu-id="be0f6-103">Список версий listItem</span><span class="sxs-lookup"><span data-stu-id="be0f6-103">List versions of a listItem</span></span>

<span data-ttu-id="be0f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be0f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be0f6-105">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="be0f6-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="be0f6-106">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="be0f6-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="be0f6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be0f6-107">Permissions</span></span>

<span data-ttu-id="be0f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be0f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="be0f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be0f6-110">Permission type</span></span>             | <span data-ttu-id="be0f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be0f6-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="be0f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be0f6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="be0f6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0f6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="be0f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be0f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be0f6-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="be0f6-115">n/a</span></span>                                         |
| <span data-ttu-id="be0f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be0f6-116">Application</span></span>                            | <span data-ttu-id="be0f6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0f6-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="be0f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0f6-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="be0f6-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0f6-119">Response</span></span>

<span data-ttu-id="be0f6-120">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be0f6-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="be0f6-121">Пример</span><span class="sxs-lookup"><span data-stu-id="be0f6-121">Example</span></span>

<span data-ttu-id="be0f6-122">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="be0f6-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="be0f6-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0f6-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="be0f6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0f6-124">Response</span></span>

<span data-ttu-id="be0f6-125">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="be0f6-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->


