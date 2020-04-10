---
title: 'СервицепринЦипалс: List ownedObjects'
description: Получение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 52ad61baddd38e49bc57755daadb8553823ac2ca
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219055"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="094cf-104">СервицепринЦипалс: List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="094cf-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="094cf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="094cf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="094cf-106">Получение списка объектов, принадлежащих servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="094cf-106">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="094cf-107">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="094cf-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="094cf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="094cf-108">Permissions</span></span>
<span data-ttu-id="094cf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="094cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="094cf-111">Permission type</span></span>      | <span data-ttu-id="094cf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="094cf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="094cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="094cf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="094cf-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="094cf-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="094cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="094cf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="094cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="094cf-116">Not supported.</span></span>    |
|<span data-ttu-id="094cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="094cf-117">Application</span></span> | <span data-ttu-id="094cf-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="094cf-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="094cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="094cf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="094cf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="094cf-120">Optional query parameters</span></span>
<span data-ttu-id="094cf-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="094cf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="094cf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="094cf-122">Request headers</span></span>
| <span data-ttu-id="094cf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="094cf-123">Name</span></span>       | <span data-ttu-id="094cf-124">Тип</span><span class="sxs-lookup"><span data-stu-id="094cf-124">Type</span></span> | <span data-ttu-id="094cf-125">Описание</span><span class="sxs-lookup"><span data-stu-id="094cf-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="094cf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="094cf-126">Authorization</span></span>  | <span data-ttu-id="094cf-127">string</span><span class="sxs-lookup"><span data-stu-id="094cf-127">string</span></span>  | <span data-ttu-id="094cf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="094cf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="094cf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="094cf-130">Request body</span></span>
<span data-ttu-id="094cf-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="094cf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="094cf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="094cf-132">Response</span></span>

<span data-ttu-id="094cf-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="094cf-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="094cf-134">Пример</span><span class="sxs-lookup"><span data-stu-id="094cf-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="094cf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="094cf-135">Request</span></span>
<span data-ttu-id="094cf-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="094cf-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="094cf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="094cf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="094cf-138">C#</span><span class="sxs-lookup"><span data-stu-id="094cf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094cf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094cf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094cf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094cf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="094cf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="094cf-141">Response</span></span>
<span data-ttu-id="094cf-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="094cf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
