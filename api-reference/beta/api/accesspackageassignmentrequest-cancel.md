---
title: 'accessPackageAssignmentRequest: отмена'
description: Отмена объектов accessPackageAssignmentRequest, которые находятся в состоянии отменяемого.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 281eebc1008f8c1c791ac6cc2694a458c86f526b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679668"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="8f274-103">accessPackageAssignmentRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="8f274-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="8f274-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f274-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)отменяйте [объекты accessPackageAssignmentRequest,](../resources/accesspackageassignmentrequest.md) которые находятся в отменяемом состоянии: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .</span><span class="sxs-lookup"><span data-stu-id="8f274-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f274-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f274-106">Permissions</span></span>
<span data-ttu-id="8f274-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f274-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f274-109">Permission type</span></span>|<span data-ttu-id="8f274-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f274-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f274-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f274-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f274-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f274-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="8f274-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f274-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f274-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f274-114">Not supported.</span></span>|
|<span data-ttu-id="8f274-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f274-115">Application</span></span>|<span data-ttu-id="8f274-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f274-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f274-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f274-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="8f274-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f274-118">Request headers</span></span>
|<span data-ttu-id="8f274-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f274-119">Name</span></span>|<span data-ttu-id="8f274-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f274-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f274-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f274-121">Authorization</span></span>|<span data-ttu-id="8f274-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f274-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f274-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f274-124">Request body</span></span>
<span data-ttu-id="8f274-125">В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8f274-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="8f274-126">Чтобы пользователь, не управляющий, отменил свой собственный запрос, запрос должен содержать **id** [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) и **запросStatus** со значением `cancelled` .</span><span class="sxs-lookup"><span data-stu-id="8f274-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="8f274-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f274-127">Response</span></span>

<span data-ttu-id="8f274-128">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="8f274-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="8f274-129">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f274-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f274-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f274-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f274-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f274-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8f274-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f274-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[<span data-ttu-id="8f274-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f274-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f274-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f274-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8f274-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f274-135">Response</span></span>
<span data-ttu-id="8f274-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f274-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

