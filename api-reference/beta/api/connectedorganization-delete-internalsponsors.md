---
title: Удаление внутреннего спонсора подключенной Организации
description: Удаление пользователя или группы из внутренних спонсоров подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de860ed2e5bc087ec14b1ee0765cc1a863724e93
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957793"
---
# <a name="remove-connected-organization-internal-sponsor"></a><span data-ttu-id="f1cea-103">Удаление внутреннего спонсора подключенной Организации</span><span class="sxs-lookup"><span data-stu-id="f1cea-103">Remove connected organization internal sponsor</span></span>

<span data-ttu-id="f1cea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1cea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1cea-105">Удаление пользователя или группы из внутренних спонсоров подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="f1cea-105">Remove a user or a group from the connected organization's internal sponsors.</span></span> <span data-ttu-id="f1cea-106">Внутренние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="f1cea-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1cea-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cea-107">Permissions</span></span>
<span data-ttu-id="f1cea-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1cea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cea-110">Permission type</span></span>      | <span data-ttu-id="f1cea-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1cea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1cea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1cea-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1cea-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1cea-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="f1cea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1cea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1cea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cea-115">Not supported.</span></span>    |
|<span data-ttu-id="f1cea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1cea-116">Application</span></span> | <span data-ttu-id="f1cea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cea-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1cea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1cea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f1cea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1cea-119">Request headers</span></span>
| <span data-ttu-id="f1cea-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f1cea-120">Name</span></span>       | <span data-ttu-id="f1cea-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f1cea-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1cea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1cea-122">Authorization</span></span>  | <span data-ttu-id="f1cea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1cea-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1cea-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1cea-125">Request body</span></span>
<span data-ttu-id="f1cea-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1cea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1cea-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1cea-127">Response</span></span>
<span data-ttu-id="f1cea-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1cea-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cea-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f1cea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1cea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1cea-131">Request</span></span>

<span data-ttu-id="f1cea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1cea-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="f1cea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1cea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f1cea-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1cea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-internalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1cea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1cea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-internalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1cea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1cea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-internalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1cea-137">Java</span><span class="sxs-lookup"><span data-stu-id="f1cea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-internalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1cea-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1cea-138">Response</span></span>

<span data-ttu-id="f1cea-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1cea-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connected organization internal sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


