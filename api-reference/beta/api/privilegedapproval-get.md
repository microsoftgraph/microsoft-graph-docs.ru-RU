---
title: Получение privilegedApproval
description: Получение свойств и связей объекта привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: dbf8611e94e07b4f0a5bea1024a59779f72c53dc
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218817"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="7d33d-103">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d33d-103">Get privilegedApproval</span></span>

<span data-ttu-id="7d33d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d33d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d33d-105">Получение свойств и связей объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="7d33d-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d33d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d33d-106">Permissions</span></span>
<span data-ttu-id="7d33d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d33d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d33d-109">Permission type</span></span>      | <span data-ttu-id="7d33d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d33d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d33d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d33d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d33d-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="7d33d-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7d33d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d33d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d33d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d33d-114">Not supported.</span></span>    |
|<span data-ttu-id="7d33d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d33d-115">Application</span></span> | <span data-ttu-id="7d33d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d33d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d33d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d33d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d33d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d33d-118">Optional query parameters</span></span>
<span data-ttu-id="7d33d-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d33d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d33d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d33d-120">Request headers</span></span>
| <span data-ttu-id="7d33d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7d33d-121">Name</span></span>      |<span data-ttu-id="7d33d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7d33d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d33d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d33d-123">Authorization</span></span>  | <span data-ttu-id="7d33d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d33d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d33d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d33d-126">Request body</span></span>
<span data-ttu-id="7d33d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d33d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d33d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d33d-128">Response</span></span>

<span data-ttu-id="7d33d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d33d-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="7d33d-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="7d33d-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7d33d-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="7d33d-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7d33d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7d33d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d33d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d33d-133">Request</span></span>
<span data-ttu-id="7d33d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d33d-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d33d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d33d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="7d33d-136">C#</span><span class="sxs-lookup"><span data-stu-id="7d33d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d33d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d33d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d33d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d33d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d33d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d33d-139">Response</span></span>
<span data-ttu-id="7d33d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d33d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
