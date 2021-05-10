---
title: 'accessPackageAssignmentRequest: отмена'
description: Отмена объектов accessPackageAssignmentRequest, которые находятся в состоянии отменяемого.
localization_priority: Normal
author: sbounouh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5079de33f7ef3c7536baf50a876a84d5ca3711b4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299562"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="2d06d-103">accessPackageAssignmentRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="2d06d-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="2d06d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d06d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d06d-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)отменяйте [объекты accessPackageAssignmentRequest,](../resources/accesspackageassignmentrequest.md) которые находятся в отменяемом состоянии: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .</span><span class="sxs-lookup"><span data-stu-id="2d06d-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d06d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d06d-106">Permissions</span></span>
<span data-ttu-id="2d06d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d06d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d06d-109">Permission type</span></span>|<span data-ttu-id="2d06d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d06d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d06d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d06d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d06d-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d06d-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="2d06d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d06d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d06d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d06d-114">Not supported.</span></span>|
|<span data-ttu-id="2d06d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d06d-115">Application</span></span>|<span data-ttu-id="2d06d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d06d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d06d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d06d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="2d06d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d06d-118">Request headers</span></span>
|<span data-ttu-id="2d06d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2d06d-119">Name</span></span>|<span data-ttu-id="2d06d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2d06d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d06d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d06d-121">Authorization</span></span>|<span data-ttu-id="2d06d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d06d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d06d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d06d-124">Request body</span></span>
<span data-ttu-id="2d06d-125">В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2d06d-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="2d06d-126">Чтобы пользователь, не управляющий, отменил свой собственный запрос, запрос должен содержать **id** [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) и **запросStatus** со значением `cancelled` .</span><span class="sxs-lookup"><span data-stu-id="2d06d-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="2d06d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d06d-127">Response</span></span>

<span data-ttu-id="2d06d-128">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2d06d-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="2d06d-129">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d06d-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d06d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d06d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d06d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d06d-131">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="2d06d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d06d-132">Response</span></span>
<span data-ttu-id="2d06d-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d06d-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

