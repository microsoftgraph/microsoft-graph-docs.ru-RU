---
title: 'identityUserFlowAttributeAssignment: setOrder'
description: Задайте порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dc9e539b56d44bcfedf5818b7be6126421fedd96
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920655"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="ae90e-103">identityUserFlowAttributeAssignment: setOrder</span><span class="sxs-lookup"><span data-stu-id="ae90e-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="ae90e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae90e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae90e-105">Задайте порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae90e-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae90e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae90e-106">Permissions</span></span>

<span data-ttu-id="ae90e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae90e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae90e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae90e-109">Permission type</span></span>|<span data-ttu-id="ae90e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae90e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae90e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae90e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae90e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae90e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ae90e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae90e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae90e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ae90e-114">Not supported</span></span>|
|<span data-ttu-id="ae90e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae90e-115">Application</span></span>|<span data-ttu-id="ae90e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae90e-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae90e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae90e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="ae90e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae90e-118">Request headers</span></span>

|<span data-ttu-id="ae90e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae90e-119">Name</span></span>|<span data-ttu-id="ae90e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae90e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae90e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae90e-121">Authorization</span></span>|<span data-ttu-id="ae90e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae90e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae90e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae90e-124">Content-Type</span></span>|<span data-ttu-id="ae90e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae90e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae90e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae90e-127">Request body</span></span>

<span data-ttu-id="ae90e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae90e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ae90e-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ae90e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ae90e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae90e-130">Parameter</span></span>|<span data-ttu-id="ae90e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae90e-131">Type</span></span>|<span data-ttu-id="ae90e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae90e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae90e-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="ae90e-133">newAssignmentOrder</span></span>|[<span data-ttu-id="ae90e-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="ae90e-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="ae90e-135">Используется для определения порядка атрибутов, собираемого в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae90e-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="ae90e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae90e-136">Response</span></span>

<span data-ttu-id="ae90e-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ae90e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ae90e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae90e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae90e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae90e-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ae90e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae90e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/userAttributeAssignments/setOrder
Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ae90e-141">C#</span><span class="sxs-lookup"><span data-stu-id="ae90e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-setorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae90e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae90e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae90e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae90e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-setorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae90e-144">Java</span><span class="sxs-lookup"><span data-stu-id="ae90e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-setorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ae90e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae90e-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
