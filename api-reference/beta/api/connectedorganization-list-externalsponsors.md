---
title: Список externalSponsors
description: Получить список внешнихSponsors connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 299a957386387b7faee6daeae8a064fe46fbd663
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872704"
---
# <a name="list-externalsponsors"></a><span data-ttu-id="61bb6-103">Список externalSponsors</span><span class="sxs-lookup"><span data-stu-id="61bb6-103">List externalSponsors</span></span>

<span data-ttu-id="61bb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61bb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61bb6-105">Получить список внешних спонсоров [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="61bb6-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s external sponsors.</span></span>  <span data-ttu-id="61bb6-106">Внешние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="61bb6-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="61bb6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61bb6-107">Permissions</span></span>

<span data-ttu-id="61bb6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61bb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61bb6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61bb6-110">Permission type</span></span>|<span data-ttu-id="61bb6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61bb6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="61bb6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61bb6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="61bb6-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61bb6-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="61bb6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61bb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61bb6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61bb6-115">Not supported.</span></span> |
| <span data-ttu-id="61bb6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61bb6-116">Application</span></span>                            | <span data-ttu-id="61bb6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61bb6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61bb6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61bb6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="61bb6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61bb6-119">Request headers</span></span>
|<span data-ttu-id="61bb6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="61bb6-120">Name</span></span>|<span data-ttu-id="61bb6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="61bb6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61bb6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61bb6-122">Authorization</span></span>|<span data-ttu-id="61bb6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61bb6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61bb6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61bb6-125">Request body</span></span>
<span data-ttu-id="61bb6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61bb6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61bb6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="61bb6-127">Response</span></span>

<span data-ttu-id="61bb6-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="61bb6-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61bb6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="61bb6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61bb6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="61bb6-130">Request</span></span>

<span data-ttu-id="61bb6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61bb6-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="61bb6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="61bb6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_externalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```
# <a name="c"></a>[<span data-ttu-id="61bb6-133">C#</span><span class="sxs-lookup"><span data-stu-id="61bb6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectedorganization-get-externalsponsors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61bb6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61bb6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectedorganization-get-externalsponsors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61bb6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61bb6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectedorganization-get-externalsponsors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61bb6-136">Java</span><span class="sxs-lookup"><span data-stu-id="61bb6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/connectedorganization-get-externalsponsors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61bb6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="61bb6-137">Response</span></span>

<span data-ttu-id="61bb6-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="61bb6-138">The following is an example of the response.</span></span>

<span data-ttu-id="61bb6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="61bb6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List externalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


