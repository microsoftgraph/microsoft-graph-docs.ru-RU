---
title: Перечисление privilegedApproval
description: Получение списка объектов привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1f6808eb2d787dd80ba17aeb02864ade3f38ce22
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314138"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="ee728-103">Перечисление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ee728-103">List privilegedApproval</span></span>

<span data-ttu-id="ee728-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee728-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee728-105">Получение списка объектов привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="ee728-105">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="ee728-106">Чтобы отфильтровать результаты запроса, используйте стандартные выражения OData ``$filter`` в URI.</span><span class="sxs-lookup"><span data-stu-id="ee728-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee728-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee728-107">Permissions</span></span>
<span data-ttu-id="ee728-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ee728-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee728-110">Permission type</span></span>      | <span data-ttu-id="ee728-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee728-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee728-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee728-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee728-113">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ee728-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee728-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee728-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee728-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee728-115">Not supported.</span></span>    |
|<span data-ttu-id="ee728-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee728-116">Application</span></span> | <span data-ttu-id="ee728-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee728-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee728-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee728-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee728-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee728-119">Optional query parameters</span></span>
<span data-ttu-id="ee728-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee728-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee728-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee728-121">Request headers</span></span>
| <span data-ttu-id="ee728-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ee728-122">Name</span></span>      |<span data-ttu-id="ee728-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ee728-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee728-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee728-124">Authorization</span></span>  | <span data-ttu-id="ee728-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee728-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee728-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee728-127">Request body</span></span>
<span data-ttu-id="ee728-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee728-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee728-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee728-129">Response</span></span>

<span data-ttu-id="ee728-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee728-130">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="ee728-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ee728-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ee728-132">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="ee728-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ee728-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ee728-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee728-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee728-134">Request</span></span>
<span data-ttu-id="ee728-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee728-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee728-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee728-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="c"></a>[<span data-ttu-id="ee728-137">C#</span><span class="sxs-lookup"><span data-stu-id="ee728-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee728-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee728-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee728-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee728-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ee728-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee728-140">Response</span></span>
<span data-ttu-id="ee728-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee728-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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