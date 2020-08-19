---
title: Добавление внешнего спонсора для подключенной Организации
description: Добавление пользователя или группы в Внешние спонсоры подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98a71e2e3e0ca5c15cb7321b2d4ae59ad5576506
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810200"
---
# <a name="add-connected-organization-external-sponsor"></a><span data-ttu-id="b3705-103">Добавление внешнего спонсора для подключенной Организации</span><span class="sxs-lookup"><span data-stu-id="b3705-103">Add connected organization external sponsor</span></span>

<span data-ttu-id="b3705-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3705-105">Добавление пользователя или группы в Внешние спонсоры подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="b3705-105">Add a user or a group to the connected organization's external sponsors.</span></span> <span data-ttu-id="b3705-106">Внешние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="b3705-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3705-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3705-107">Permissions</span></span>
<span data-ttu-id="b3705-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3705-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3705-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3705-110">Permission type</span></span>      | <span data-ttu-id="b3705-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3705-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3705-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3705-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3705-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3705-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="b3705-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3705-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3705-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3705-115">Not supported.</span></span>    |
|<span data-ttu-id="b3705-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3705-116">Application</span></span> | <span data-ttu-id="b3705-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3705-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3705-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3705-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b3705-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3705-119">Request headers</span></span>
| <span data-ttu-id="b3705-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b3705-120">Name</span></span>       | <span data-ttu-id="b3705-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b3705-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3705-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3705-122">Authorization</span></span>  | <span data-ttu-id="b3705-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3705-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3705-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3705-125">Content-type</span></span> | <span data-ttu-id="b3705-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3705-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3705-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3705-128">Request body</span></span>
<span data-ttu-id="b3705-129">В теле запроса добавьте представление ссылки на объект добавляемого [пользователя](../resources/user.md) или [группы](../resources/group.md) в виде `@odata.id` свойства с полным URI пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="b3705-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="b3705-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3705-130">Response</span></span>
<span data-ttu-id="b3705-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3705-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3705-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b3705-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3705-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3705-134">Request</span></span>

<span data-ttu-id="b3705-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3705-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3705-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3705-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b3705-137">C#</span><span class="sxs-lookup"><span data-stu-id="b3705-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3705-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3705-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3705-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3705-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3705-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3705-140">Response</span></span>

<span data-ttu-id="b3705-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3705-141">The following is an example of the response.</span></span>

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
  "description": "Create connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
