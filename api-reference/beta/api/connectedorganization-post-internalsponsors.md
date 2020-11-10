---
title: Добавление внутреннего спонсора для подключенной Организации
description: Добавление пользователя или группы в внутренние спонсоры подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c63c25d3c08b717977c2c75ce7b4fe737cf2eef0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957639"
---
# <a name="add-connected-organization-internal-sponsor"></a><span data-ttu-id="386ed-103">Добавление внутреннего спонсора для подключенной Организации</span><span class="sxs-lookup"><span data-stu-id="386ed-103">Add connected organization internal sponsor</span></span>

<span data-ttu-id="386ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="386ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="386ed-105">Добавление пользователя или группы в внутренние спонсоры подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="386ed-105">Add a user or a group to the connected organization's internal sponsors.</span></span> <span data-ttu-id="386ed-106">Внутренние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="386ed-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="386ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="386ed-107">Permissions</span></span>
<span data-ttu-id="386ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="386ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="386ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="386ed-110">Permission type</span></span>      | <span data-ttu-id="386ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="386ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="386ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="386ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="386ed-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386ed-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="386ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="386ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="386ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="386ed-115">Not supported.</span></span>    |
|<span data-ttu-id="386ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="386ed-116">Application</span></span> | <span data-ttu-id="386ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="386ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="386ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="386ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="386ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="386ed-119">Request headers</span></span>
| <span data-ttu-id="386ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="386ed-120">Name</span></span>       | <span data-ttu-id="386ed-121">Описание</span><span class="sxs-lookup"><span data-stu-id="386ed-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="386ed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="386ed-122">Authorization</span></span>  | <span data-ttu-id="386ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="386ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="386ed-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="386ed-125">Content-type</span></span> | <span data-ttu-id="386ed-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="386ed-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="386ed-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="386ed-128">Request body</span></span>
<span data-ttu-id="386ed-129">В теле запроса добавьте представление ссылки на объект добавляемого [пользователя](../resources/user.md) или [группы](../resources/group.md) в виде `@odata.id` свойства с полным URI пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="386ed-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="386ed-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="386ed-130">Response</span></span>
<span data-ttu-id="386ed-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="386ed-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="386ed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="386ed-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="386ed-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="386ed-134">Request</span></span>

<span data-ttu-id="386ed-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="386ed-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="386ed-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="386ed-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="386ed-137">C#</span><span class="sxs-lookup"><span data-stu-id="386ed-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-internalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="386ed-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="386ed-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-internalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="386ed-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="386ed-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-internalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="386ed-140">Java</span><span class="sxs-lookup"><span data-stu-id="386ed-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-internalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="386ed-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="386ed-141">Response</span></span>

<span data-ttu-id="386ed-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="386ed-142">The following is an example of the response.</span></span>

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


