---
title: Перечисление privilegedApproval
description: Получение списка объектов привилежедаппровал.
localization_priority: Normal
ms.openlocfilehash: b2b9c71ec45033cb9fbf209cdcc97a20fd2f891e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445088"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="7975e-103">Перечисление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7975e-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7975e-104">Получение списка объектов привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="7975e-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="7975e-105">Чтобы отфильтровать результаты запроса, используйте стандартные выражения OData ``$filter`` в URI.</span><span class="sxs-lookup"><span data-stu-id="7975e-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="7975e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7975e-106">Permissions</span></span>
<span data-ttu-id="7975e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7975e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7975e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7975e-109">Permission type</span></span>      | <span data-ttu-id="7975e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7975e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7975e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7975e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7975e-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="7975e-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7975e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7975e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7975e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7975e-114">Not supported.</span></span>    |
|<span data-ttu-id="7975e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7975e-115">Application</span></span> | <span data-ttu-id="7975e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7975e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7975e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7975e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7975e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7975e-118">Optional query parameters</span></span>
<span data-ttu-id="7975e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7975e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7975e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7975e-120">Request headers</span></span>
| <span data-ttu-id="7975e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7975e-121">Name</span></span>      |<span data-ttu-id="7975e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7975e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7975e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7975e-123">Authorization</span></span>  | <span data-ttu-id="7975e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7975e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7975e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7975e-126">Request body</span></span>
<span data-ttu-id="7975e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7975e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7975e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7975e-128">Response</span></span>

<span data-ttu-id="7975e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7975e-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="7975e-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="7975e-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7975e-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="7975e-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7975e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7975e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7975e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7975e-133">Request</span></span>
<span data-ttu-id="7975e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7975e-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7975e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7975e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7975e-136">C#</span><span class="sxs-lookup"><span data-stu-id="7975e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7975e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7975e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7975e-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7975e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7975e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7975e-139">Response</span></span>
<span data-ttu-id="7975e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7975e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
