---
title: Список directoryRoleTemplate
description: Получение списка объектов directoryRoleTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6d7dea5863052b72d1112f631a319a3e870ccdb
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727007"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="43123-103">Список directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="43123-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="43123-104">Получение списка объектов directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="43123-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="43123-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43123-105">Permissions</span></span>
<span data-ttu-id="43123-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="43123-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43123-108">Permission type</span></span>      | <span data-ttu-id="43123-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43123-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43123-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43123-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43123-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="43123-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43123-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43123-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43123-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43123-113">Not supported.</span></span>    |
|<span data-ttu-id="43123-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43123-114">Application</span></span> | <span data-ttu-id="43123-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="43123-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43123-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43123-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43123-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43123-117">Optional query parameters</span></span>
<span data-ttu-id="43123-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="43123-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43123-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43123-119">Request headers</span></span>
| <span data-ttu-id="43123-120">Имя</span><span class="sxs-lookup"><span data-stu-id="43123-120">Name</span></span>       | <span data-ttu-id="43123-121">Тип</span><span class="sxs-lookup"><span data-stu-id="43123-121">Type</span></span> | <span data-ttu-id="43123-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43123-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="43123-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43123-123">Authorization</span></span>  | <span data-ttu-id="43123-124">string</span><span class="sxs-lookup"><span data-stu-id="43123-124">string</span></span>  | <span data-ttu-id="43123-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43123-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43123-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43123-127">Request body</span></span>
<span data-ttu-id="43123-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43123-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43123-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="43123-129">Response</span></span>

<span data-ttu-id="43123-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="43123-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43123-131">Пример</span><span class="sxs-lookup"><span data-stu-id="43123-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43123-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="43123-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="43123-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="43123-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43123-134">C#</span><span class="sxs-lookup"><span data-stu-id="43123-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43123-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43123-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43123-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="43123-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="43123-137">Java</span><span class="sxs-lookup"><span data-stu-id="43123-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="43123-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="43123-138">Response</span></span>
<span data-ttu-id="43123-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43123-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
