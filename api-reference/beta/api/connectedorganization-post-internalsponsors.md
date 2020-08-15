---
title: Добавление внутреннего спонсора для подключенной Организации
description: Добавление пользователя или группы в внутренние спонсоры подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e12ff2bf8b0973243dbef6ddd023a0e492832caa
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757484"
---
# <a name="add-connected-organization-internal-sponsor"></a><span data-ttu-id="64f78-103">Добавление внутреннего спонсора для подключенной Организации</span><span class="sxs-lookup"><span data-stu-id="64f78-103">Add connected organization internal sponsor</span></span>

<span data-ttu-id="64f78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f78-105">Добавление пользователя или группы в внутренние спонсоры подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="64f78-105">Add a user or a group to the connected organization's internal sponsors.</span></span> <span data-ttu-id="64f78-106">Внутренние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="64f78-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="64f78-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64f78-107">Permissions</span></span>
<span data-ttu-id="64f78-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f78-110">Permission type</span></span>      | <span data-ttu-id="64f78-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64f78-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f78-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="64f78-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f78-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="64f78-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f78-115">Not supported.</span></span>    |
|<span data-ttu-id="64f78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64f78-116">Application</span></span> | <span data-ttu-id="64f78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f78-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64f78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f78-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="64f78-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64f78-119">Request headers</span></span>
| <span data-ttu-id="64f78-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64f78-120">Name</span></span>       | <span data-ttu-id="64f78-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64f78-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64f78-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f78-122">Authorization</span></span>  | <span data-ttu-id="64f78-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f78-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64f78-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64f78-125">Content-type</span></span> | <span data-ttu-id="64f78-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f78-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64f78-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64f78-128">Request body</span></span>
<span data-ttu-id="64f78-129">В теле запроса добавьте представление ссылки на объект добавляемого [пользователя](../resources/user.md) или [группы](../resources/group.md) в виде `@odata.id` свойства с полным URI пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="64f78-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="64f78-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f78-130">Response</span></span>
<span data-ttu-id="64f78-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64f78-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f78-133">Пример</span><span class="sxs-lookup"><span data-stu-id="64f78-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f78-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f78-134">Request</span></span>

<span data-ttu-id="64f78-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64f78-135">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="64f78-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f78-136">Response</span></span>

<span data-ttu-id="64f78-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64f78-137">The following is an example of the response.</span></span>

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
