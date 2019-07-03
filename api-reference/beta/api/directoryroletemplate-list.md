---
title: Список directoryRoleTemplate
description: Получение списка объектов directoryroletemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c92a872a2db9cace2a70625f17cce8d4c394959
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436860"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="29906-103">Список directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="29906-103">List directoryRoleTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29906-104">Получение списка объектов directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="29906-104">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="29906-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29906-105">Permissions</span></span>
<span data-ttu-id="29906-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29906-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29906-108">Permission type</span></span>      | <span data-ttu-id="29906-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29906-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29906-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29906-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29906-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29906-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29906-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29906-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29906-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29906-113">Not supported.</span></span>    |
|<span data-ttu-id="29906-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29906-114">Application</span></span> | <span data-ttu-id="29906-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29906-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29906-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29906-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29906-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29906-117">Optional query parameters</span></span>
<span data-ttu-id="29906-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="29906-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="29906-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29906-119">Request headers</span></span>
| <span data-ttu-id="29906-120">Имя</span><span class="sxs-lookup"><span data-stu-id="29906-120">Name</span></span>       | <span data-ttu-id="29906-121">Тип</span><span class="sxs-lookup"><span data-stu-id="29906-121">Type</span></span> | <span data-ttu-id="29906-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29906-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29906-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29906-123">Authorization</span></span>  | <span data-ttu-id="29906-124">string</span><span class="sxs-lookup"><span data-stu-id="29906-124">string</span></span>  | <span data-ttu-id="29906-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29906-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29906-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29906-127">Request body</span></span>
<span data-ttu-id="29906-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29906-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29906-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29906-129">Response</span></span>

<span data-ttu-id="29906-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29906-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29906-131">Пример</span><span class="sxs-lookup"><span data-stu-id="29906-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29906-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29906-132">Request</span></span>
<span data-ttu-id="29906-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29906-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29906-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="29906-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29906-135">C#</span><span class="sxs-lookup"><span data-stu-id="29906-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29906-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="29906-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29906-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="29906-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="29906-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="29906-138">Response</span></span>
<span data-ttu-id="29906-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29906-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

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
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
