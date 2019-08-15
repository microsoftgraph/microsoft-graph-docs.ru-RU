---
title: 'Привилежедролеассигнмент: Макилигибле'
description: Выполнение назначения ролей как соответствующего требованиям. Если назначение роли уже доступно перед вызовом, оно ничего не делает. Если назначение роли является необратимым, а запрашивающий отличается от конечного пользователя, назначение роли станет доступным, и роль будет отключена для целевого пользователя. Если запрашивающей стороны является целевой пользователь, а роль является администратором безопасности или привилегированным администратором ролей, роль будет активирована с истечением срока действия по умолчанию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: db1de3f84ce06c5caeb9a3b18884f92132c39da6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412707"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="0688d-106">Привилежедролеассигнмент: Макилигибле</span><span class="sxs-lookup"><span data-stu-id="0688d-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0688d-107">Выполнение назначения ролей как соответствующего требованиям.</span><span class="sxs-lookup"><span data-stu-id="0688d-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="0688d-108">Если назначение роли уже доступно перед вызовом, оно ничего не делает.</span><span class="sxs-lookup"><span data-stu-id="0688d-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="0688d-109">Если назначение роли является необратимым, а запрашивающий отличается от конечного пользователя, назначение роли станет доступным, и роль будет отключена для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0688d-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="0688d-110">Если запрашивающей стороны является целевой пользователь, а роль является администратором безопасности или привилегированным администратором ролей, роль будет активирована с истечением срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0688d-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="0688d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0688d-111">Permissions</span></span>
<span data-ttu-id="0688d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0688d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0688d-114">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="0688d-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="0688d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0688d-115">Permission type</span></span>      | <span data-ttu-id="0688d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0688d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0688d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0688d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0688d-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0688d-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0688d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0688d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0688d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0688d-120">Not supported.</span></span>    |
|<span data-ttu-id="0688d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0688d-121">Application</span></span> | <span data-ttu-id="0688d-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0688d-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0688d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0688d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="0688d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0688d-124">Request headers</span></span>
| <span data-ttu-id="0688d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0688d-125">Name</span></span>       | <span data-ttu-id="0688d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0688d-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0688d-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0688d-127">Authorization</span></span>  | <span data-ttu-id="0688d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0688d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0688d-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0688d-130">Request body</span></span>
<span data-ttu-id="0688d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0688d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0688d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0688d-132">Response</span></span>

<span data-ttu-id="0688d-133">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0688d-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="0688d-134">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="0688d-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0688d-135">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="0688d-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="0688d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="0688d-136">Example</span></span>
<span data-ttu-id="0688d-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0688d-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0688d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0688d-138">Request</span></span>
<span data-ttu-id="0688d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0688d-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0688d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0688d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0688d-141">C#</span><span class="sxs-lookup"><span data-stu-id="0688d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0688d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0688d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0688d-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0688d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0688d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0688d-144">Response</span></span>
<span data-ttu-id="0688d-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0688d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
