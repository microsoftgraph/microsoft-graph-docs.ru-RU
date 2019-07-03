---
title: Получение privilegedApproval
description: Получение свойств и связей объекта привилежедаппровал.
localization_priority: Normal
ms.openlocfilehash: 4e964d51ee930814565f5e8eadaff85e4077e24f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445095"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="520cf-103">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="520cf-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="520cf-104">Получение свойств и связей объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="520cf-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="520cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="520cf-105">Permissions</span></span>
<span data-ttu-id="520cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="520cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="520cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="520cf-108">Permission type</span></span>      | <span data-ttu-id="520cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="520cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="520cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="520cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="520cf-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="520cf-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="520cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="520cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520cf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="520cf-113">Not supported.</span></span>    |
|<span data-ttu-id="520cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="520cf-114">Application</span></span> | <span data-ttu-id="520cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="520cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="520cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="520cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="520cf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="520cf-117">Optional query parameters</span></span>
<span data-ttu-id="520cf-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="520cf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="520cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="520cf-119">Request headers</span></span>
| <span data-ttu-id="520cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="520cf-120">Name</span></span>      |<span data-ttu-id="520cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="520cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="520cf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="520cf-122">Authorization</span></span>  | <span data-ttu-id="520cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="520cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="520cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="520cf-125">Request body</span></span>
<span data-ttu-id="520cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="520cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="520cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="520cf-127">Response</span></span>

<span data-ttu-id="520cf-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="520cf-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="520cf-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="520cf-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="520cf-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="520cf-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="520cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="520cf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="520cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="520cf-132">Request</span></span>
<span data-ttu-id="520cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="520cf-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="520cf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="520cf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="520cf-135">C#</span><span class="sxs-lookup"><span data-stu-id="520cf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="520cf-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="520cf-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="520cf-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="520cf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="520cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="520cf-138">Response</span></span>
<span data-ttu-id="520cf-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="520cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
