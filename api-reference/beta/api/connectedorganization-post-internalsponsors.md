---
title: Добавление внутреннего спонсора подключенной организации
description: Добавьте пользователя или группу во внутренние спонсоры подключенной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ebdc00ed51ed63e4e22794c98b916fd22db9b2a2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437436"
---
# <a name="add-connected-organization-internal-sponsor"></a><span data-ttu-id="feaba-103">Добавление внутреннего спонсора подключенной организации</span><span class="sxs-lookup"><span data-stu-id="feaba-103">Add connected organization internal sponsor</span></span>

<span data-ttu-id="feaba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feaba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feaba-105">Добавьте пользователя или группу во внутренние спонсоры связанной организации.</span><span class="sxs-lookup"><span data-stu-id="feaba-105">Add a user or a group to the connected organization's internal sponsors.</span></span> <span data-ttu-id="feaba-106">Внутренние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой связанной организации.</span><span class="sxs-lookup"><span data-stu-id="feaba-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="feaba-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="feaba-107">Permissions</span></span>
<span data-ttu-id="feaba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feaba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feaba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="feaba-110">Permission type</span></span>      | <span data-ttu-id="feaba-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="feaba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feaba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="feaba-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="feaba-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feaba-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="feaba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feaba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feaba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feaba-115">Not supported.</span></span>    |
|<span data-ttu-id="feaba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="feaba-116">Application</span></span> | <span data-ttu-id="feaba-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feaba-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="feaba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="feaba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="feaba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="feaba-119">Request headers</span></span>
| <span data-ttu-id="feaba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="feaba-120">Name</span></span>       | <span data-ttu-id="feaba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="feaba-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="feaba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="feaba-122">Authorization</span></span>  | <span data-ttu-id="feaba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="feaba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="feaba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="feaba-125">Content-type</span></span> | <span data-ttu-id="feaba-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="feaba-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="feaba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="feaba-128">Request body</span></span>
<span data-ttu-id="feaba-129">В тексте запроса в качестве свойства с [](../resources/user.md) полным [](../resources/group.md) URI пользователя или группы необходимо предоставить представление JSON ссылки на добавленный объект пользователя или `@odata.id` группы.</span><span class="sxs-lookup"><span data-stu-id="feaba-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="feaba-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="feaba-130">Response</span></span>
<span data-ttu-id="feaba-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="feaba-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feaba-133">Пример</span><span class="sxs-lookup"><span data-stu-id="feaba-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="feaba-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="feaba-134">Request</span></span>

<span data-ttu-id="feaba-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="feaba-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="feaba-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="feaba-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_internalsponsor_from_connectedorganization"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="feaba-137">C#</span><span class="sxs-lookup"><span data-stu-id="feaba-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-internalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="feaba-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feaba-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-internalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="feaba-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="feaba-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-internalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="feaba-140">Java</span><span class="sxs-lookup"><span data-stu-id="feaba-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-internalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="feaba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="feaba-141">Response</span></span>

<span data-ttu-id="feaba-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="feaba-142">The following is an example of the response.</span></span>

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
  "description": "Create connected organization internal sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


