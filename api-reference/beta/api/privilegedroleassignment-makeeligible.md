---
title: 'Привилежедролеассигнмент: Макилигибле'
description: Сделайте назначение роли доступным.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 2f0c4f4f9126614e3aa228c0d05480b548664958
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035058"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="a7c23-103">Привилежедролеассигнмент: Макилигибле</span><span class="sxs-lookup"><span data-stu-id="a7c23-103">privilegedRoleAssignment: makeEligible</span></span>

<span data-ttu-id="a7c23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c23-105">Сделайте назначение роли доступным.</span><span class="sxs-lookup"><span data-stu-id="a7c23-105">Make the role assignment eligible.</span></span> <span data-ttu-id="a7c23-106">Если назначение роли уже доступно перед вызовом, оно ничего не делает.</span><span class="sxs-lookup"><span data-stu-id="a7c23-106">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="a7c23-107">Если назначение роли является необратимым, а запрашивающий отличается от конечного пользователя, назначение роли станет доступным, и роль будет отключена для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7c23-107">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="a7c23-108">Если запрашивающей стороны является целевой пользователь, а роль является администратором безопасности или привилегированным администратором ролей, роль будет активирована с истечением срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a7c23-108">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7c23-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c23-109">Permissions</span></span>
<span data-ttu-id="a7c23-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a7c23-112">Запрашивающая сторона должна иметь _привилегированную роль администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="a7c23-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="a7c23-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c23-113">Permission type</span></span>      | <span data-ttu-id="a7c23-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7c23-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7c23-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7c23-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a7c23-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7c23-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7c23-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7c23-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7c23-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7c23-118">Not supported.</span></span>    |
|<span data-ttu-id="a7c23-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7c23-119">Application</span></span> | <span data-ttu-id="a7c23-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7c23-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7c23-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7c23-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="a7c23-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7c23-122">Request headers</span></span>
| <span data-ttu-id="a7c23-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a7c23-123">Name</span></span>       | <span data-ttu-id="a7c23-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a7c23-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7c23-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7c23-125">Authorization</span></span>  | <span data-ttu-id="a7c23-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7c23-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7c23-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7c23-128">Request body</span></span>
<span data-ttu-id="a7c23-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7c23-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7c23-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c23-130">Response</span></span>

<span data-ttu-id="a7c23-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7c23-131">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a7c23-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="a7c23-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a7c23-133">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="a7c23-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a7c23-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a7c23-134">Example</span></span>
<span data-ttu-id="a7c23-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a7c23-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a7c23-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7c23-136">Request</span></span>
<span data-ttu-id="a7c23-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7c23-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7c23-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c23-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="c"></a>[<span data-ttu-id="a7c23-139">C#</span><span class="sxs-lookup"><span data-stu-id="a7c23-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7c23-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7c23-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7c23-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7c23-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a7c23-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c23-142">Response</span></span>
<span data-ttu-id="a7c23-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7c23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


