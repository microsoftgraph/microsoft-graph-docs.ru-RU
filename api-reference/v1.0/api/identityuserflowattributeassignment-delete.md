---
title: Удаление userAttributeAssignment
description: Удаление объекта identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8dab44862a1859851a4c3fb9b52dcd8f3692e8c1
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920779"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="82bcf-103">Удаление userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="82bcf-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="82bcf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82bcf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82bcf-105">Удаление [объекта identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="82bcf-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82bcf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82bcf-106">Permissions</span></span>

<span data-ttu-id="82bcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82bcf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82bcf-109">Permission type</span></span>|<span data-ttu-id="82bcf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82bcf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82bcf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82bcf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82bcf-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bcf-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="82bcf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82bcf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82bcf-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="82bcf-114">Not supported</span></span>|
|<span data-ttu-id="82bcf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82bcf-115">Application</span></span>|<span data-ttu-id="82bcf-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bcf-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82bcf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82bcf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="82bcf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82bcf-118">Request headers</span></span>

|<span data-ttu-id="82bcf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="82bcf-119">Name</span></span>|<span data-ttu-id="82bcf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="82bcf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82bcf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82bcf-121">Authorization</span></span>|<span data-ttu-id="82bcf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82bcf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82bcf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82bcf-124">Request body</span></span>

<span data-ttu-id="82bcf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82bcf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82bcf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="82bcf-126">Response</span></span>

<span data-ttu-id="82bcf-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82bcf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="82bcf-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="82bcf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82bcf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="82bcf-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="82bcf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="82bcf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2xidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```
# <a name="c"></a>[<span data-ttu-id="82bcf-131">C#</span><span class="sxs-lookup"><span data-stu-id="82bcf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2xidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82bcf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82bcf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2xidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82bcf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82bcf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2xidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82bcf-134">Java</span><span class="sxs-lookup"><span data-stu-id="82bcf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2xidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82bcf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="82bcf-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
