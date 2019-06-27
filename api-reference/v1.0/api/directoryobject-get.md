---
title: Получение объекта DirectoryObject
description: Получение свойств и связей объекта directoryObject.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ecec08b7c27008596ddc973326e98658f519b73
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273656"
---
# <a name="get-directoryobject"></a><span data-ttu-id="35b3d-103">Получение объекта DirectoryObject</span><span class="sxs-lookup"><span data-stu-id="35b3d-103">Get directoryObject</span></span>

<span data-ttu-id="35b3d-104">Получение свойств и связей объекта directoryObject.</span><span class="sxs-lookup"><span data-stu-id="35b3d-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="35b3d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35b3d-105">Permissions</span></span>
<span data-ttu-id="35b3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35b3d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35b3d-108">Permission type</span></span>      | <span data-ttu-id="35b3d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35b3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35b3d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35b3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="35b3d-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35b3d-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35b3d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35b3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35b3d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b3d-113">Not supported.</span></span>    |
|<span data-ttu-id="35b3d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35b3d-114">Application</span></span> | <span data-ttu-id="35b3d-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="35b3d-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35b3d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35b3d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35b3d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35b3d-117">Optional query parameters</span></span>
<span data-ttu-id="35b3d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35b3d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35b3d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35b3d-119">Request headers</span></span>
| <span data-ttu-id="35b3d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="35b3d-120">Name</span></span>       | <span data-ttu-id="35b3d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="35b3d-121">Type</span></span> | <span data-ttu-id="35b3d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35b3d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35b3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35b3d-123">Authorization</span></span>  | <span data-ttu-id="35b3d-124">string</span><span class="sxs-lookup"><span data-stu-id="35b3d-124">string</span></span>  | <span data-ttu-id="35b3d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35b3d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35b3d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35b3d-127">Request body</span></span>
<span data-ttu-id="35b3d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35b3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35b3d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="35b3d-129">Response</span></span>

<span data-ttu-id="35b3d-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35b3d-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35b3d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35b3d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35b3d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35b3d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="35b3d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="35b3d-133">Response</span></span>
<span data-ttu-id="35b3d-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35b3d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="35b3d-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="35b3d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="35b3d-137">C#</span><span class="sxs-lookup"><span data-stu-id="35b3d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35b3d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35b3d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryobject-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="35b3d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35b3d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryobject-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
