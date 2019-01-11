---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 'Получение предыдущей версии элемента списка: API SharePoint'
localization_priority: Normal
ms.openlocfilehash: 7f009eb006e44dd2f8e25052b0326ffc92243c7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881608"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="6ee31-102">Получение ресурса ListItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="6ee31-102">Get a ListItemVersion resource (preview)</span></span>

> <span data-ttu-id="6ee31-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ee31-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ee31-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ee31-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ee31-105">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="6ee31-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ee31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee31-106">Permissions</span></span>

<span data-ttu-id="6ee31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6ee31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee31-109">Permission type</span></span>             | <span data-ttu-id="6ee31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ee31-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6ee31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ee31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ee31-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee31-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="6ee31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ee31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee31-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="6ee31-114">n/a</span></span>                                         |
| <span data-ttu-id="6ee31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ee31-115">Application</span></span>                            | <span data-ttu-id="6ee31-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee31-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="6ee31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ee31-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="6ee31-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee31-118">Response</span></span>

<span data-ttu-id="6ee31-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ee31-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="6ee31-120">Пример</span><span class="sxs-lookup"><span data-stu-id="6ee31-120">Example</span></span>

<span data-ttu-id="6ee31-121">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="6ee31-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="6ee31-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ee31-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="6ee31-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee31-123">Response</span></span>

<span data-ttu-id="6ee31-124">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="6ee31-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
