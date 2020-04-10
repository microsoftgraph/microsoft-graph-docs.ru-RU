---
title: Список servicePrincipal memberOf
description: Получение групп и ролей каталогов, непосредственным участником которых является данный участник службы. Эта операция не является транзитивной.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 50b5e26d9deb461ac672b7529450e092055824fd
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219069"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="d0a6a-104">Список servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="d0a6a-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="d0a6a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0a6a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0a6a-106">Получение групп и ролей каталогов, непосредственным участником которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-106">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="d0a6a-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0a6a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0a6a-108">Permissions</span></span>

<span data-ttu-id="d0a6a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0a6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0a6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0a6a-111">Permission type</span></span>      | <span data-ttu-id="d0a6a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0a6a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0a6a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0a6a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d0a6a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0a6a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0a6a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0a6a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0a6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-116">Not supported.</span></span>    |
|<span data-ttu-id="d0a6a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0a6a-117">Application</span></span> | <span data-ttu-id="d0a6a-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a6a-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d0a6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0a6a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0a6a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d0a6a-120">Optional query parameters</span></span>

<span data-ttu-id="d0a6a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0a6a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0a6a-122">Request headers</span></span>
| <span data-ttu-id="d0a6a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d0a6a-123">Name</span></span>       | <span data-ttu-id="d0a6a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d0a6a-124">Type</span></span> | <span data-ttu-id="d0a6a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d0a6a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0a6a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0a6a-126">Authorization</span></span>  | <span data-ttu-id="d0a6a-127">string</span><span class="sxs-lookup"><span data-stu-id="d0a6a-127">string</span></span>  | <span data-ttu-id="d0a6a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0a6a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0a6a-130">Request body</span></span>
<span data-ttu-id="d0a6a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0a6a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0a6a-132">Response</span></span>

<span data-ttu-id="d0a6a-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0a6a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d0a6a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0a6a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0a6a-135">Request</span></span>

<span data-ttu-id="d0a6a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0a6a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0a6a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="d0a6a-138">C#</span><span class="sxs-lookup"><span data-stu-id="d0a6a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0a6a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0a6a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0a6a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0a6a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0a6a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0a6a-141">Response</span></span>

<span data-ttu-id="d0a6a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0a6a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
