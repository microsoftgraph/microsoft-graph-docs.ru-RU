---
author: JeremyKelley
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
ms.date: 09/10/2017
title: Получение предыдущей версии записи списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 731a6b2a71fd03790e447dfb331c7cf4e6f5f482
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972030"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="36caa-103">Создание списка версий элемента ListItem (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="36caa-103">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="36caa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36caa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36caa-105">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="36caa-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="36caa-106">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="36caa-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="36caa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36caa-107">Permissions</span></span>

<span data-ttu-id="36caa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="36caa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36caa-110">Permission type</span></span>             | <span data-ttu-id="36caa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36caa-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="36caa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36caa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="36caa-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36caa-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="36caa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36caa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36caa-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="36caa-115">n/a</span></span>                                         |
| <span data-ttu-id="36caa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36caa-116">Application</span></span>                            | <span data-ttu-id="36caa-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36caa-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="36caa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36caa-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="36caa-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="36caa-119">Response</span></span>

<span data-ttu-id="36caa-120">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36caa-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="36caa-121">Пример</span><span class="sxs-lookup"><span data-stu-id="36caa-121">Example</span></span>

<span data-ttu-id="36caa-122">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="36caa-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="36caa-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36caa-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="36caa-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="36caa-124">Response</span></span>

<span data-ttu-id="36caa-125">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="36caa-125">This returns a collection of versions:</span></span>

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


