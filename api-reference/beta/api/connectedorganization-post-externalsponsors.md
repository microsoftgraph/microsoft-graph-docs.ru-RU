---
title: Добавление внешнего спонсора подключенной организации
description: Добавьте пользователя или группу к внешним спонсорам подключенной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 38332f46b5215989f0739450d0efef155058b443
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786161"
---
# <a name="add-connected-organization-external-sponsor"></a><span data-ttu-id="336b1-103">Добавление внешнего спонсора подключенной организации</span><span class="sxs-lookup"><span data-stu-id="336b1-103">Add connected organization external sponsor</span></span>

<span data-ttu-id="336b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="336b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="336b1-105">Добавьте пользователя или группу к внешним спонсорам подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="336b1-105">Add a user or a group to the connected organization's external sponsors.</span></span> <span data-ttu-id="336b1-106">Внешние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой связанной организации.</span><span class="sxs-lookup"><span data-stu-id="336b1-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="336b1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="336b1-107">Permissions</span></span>
<span data-ttu-id="336b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="336b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="336b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="336b1-110">Permission type</span></span>      | <span data-ttu-id="336b1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="336b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="336b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="336b1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="336b1-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="336b1-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="336b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="336b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="336b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="336b1-115">Not supported.</span></span>    |
|<span data-ttu-id="336b1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="336b1-116">Application</span></span> | <span data-ttu-id="336b1-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="336b1-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="336b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="336b1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="336b1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="336b1-119">Request headers</span></span>
| <span data-ttu-id="336b1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="336b1-120">Name</span></span>       | <span data-ttu-id="336b1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="336b1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="336b1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="336b1-122">Authorization</span></span>  | <span data-ttu-id="336b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="336b1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="336b1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="336b1-125">Content-type</span></span> | <span data-ttu-id="336b1-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="336b1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="336b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="336b1-128">Request body</span></span>
<span data-ttu-id="336b1-129">В тексте запроса в качестве свойства с [](../resources/user.md) полным [](../resources/group.md) URI пользователя или группы необходимо предоставить представление JSON ссылки на добавленный объект пользователя или `@odata.id` группы.</span><span class="sxs-lookup"><span data-stu-id="336b1-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="336b1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="336b1-130">Response</span></span>
<span data-ttu-id="336b1-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="336b1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="336b1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="336b1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="336b1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="336b1-134">Request</span></span>

<span data-ttu-id="336b1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="336b1-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="336b1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="336b1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalsponsor_from_connectedorganization"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="336b1-137">C#</span><span class="sxs-lookup"><span data-stu-id="336b1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="336b1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="336b1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="336b1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="336b1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="336b1-140">Java</span><span class="sxs-lookup"><span data-stu-id="336b1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="336b1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="336b1-141">Response</span></span>

<span data-ttu-id="336b1-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="336b1-142">The following is an example of the response.</span></span>

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
  "description": "Create connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


