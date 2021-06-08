---
title: Удаление внешнего спонсора подключенной организации
description: Удалите пользователя или группу из внешних спонсоров подключенной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 936c91f5ebd3bff0af8ec25a4ce542707e04227d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786512"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="2418f-103">Удаление внешнего спонсора подключенной организации</span><span class="sxs-lookup"><span data-stu-id="2418f-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="2418f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2418f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2418f-105">Удалите пользователя или группу из внешних спонсоров подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="2418f-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="2418f-106">Внешние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой связанной организации.</span><span class="sxs-lookup"><span data-stu-id="2418f-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="2418f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2418f-107">Permissions</span></span>
<span data-ttu-id="2418f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2418f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2418f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2418f-110">Permission type</span></span>      | <span data-ttu-id="2418f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2418f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2418f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2418f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2418f-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2418f-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="2418f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2418f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2418f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2418f-115">Not supported.</span></span>    |
|<span data-ttu-id="2418f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2418f-116">Application</span></span> | <span data-ttu-id="2418f-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2418f-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2418f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2418f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2418f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2418f-119">Request headers</span></span>
| <span data-ttu-id="2418f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2418f-120">Name</span></span>       | <span data-ttu-id="2418f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2418f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2418f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2418f-122">Authorization</span></span>  | <span data-ttu-id="2418f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2418f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2418f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2418f-125">Request body</span></span>
<span data-ttu-id="2418f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2418f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2418f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2418f-127">Response</span></span>
<span data-ttu-id="2418f-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2418f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2418f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2418f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2418f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2418f-131">Request</span></span>

<span data-ttu-id="2418f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2418f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2418f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2418f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="2418f-134">C#</span><span class="sxs-lookup"><span data-stu-id="2418f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2418f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2418f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2418f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2418f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2418f-137">Java</span><span class="sxs-lookup"><span data-stu-id="2418f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2418f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2418f-138">Response</span></span>

<span data-ttu-id="2418f-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2418f-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


