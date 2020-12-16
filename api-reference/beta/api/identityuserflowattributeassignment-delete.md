---
title: Удаление userAttributeAssignment
description: Удаление объекта identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7b83e264c05c3636f21237529c85b567a5eea8d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689559"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="1bb37-103">Удаление userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1bb37-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="1bb37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bb37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bb37-105">Удаление объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1bb37-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bb37-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bb37-106">Permissions</span></span>

<span data-ttu-id="1bb37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bb37-109">Permission type</span></span>|<span data-ttu-id="1bb37-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bb37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb37-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bb37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb37-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb37-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1bb37-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bb37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb37-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1bb37-114">Not supported</span></span>|
|<span data-ttu-id="1bb37-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bb37-115">Application</span></span>|<span data-ttu-id="1bb37-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb37-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb37-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bb37-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1bb37-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bb37-118">Request headers</span></span>

|<span data-ttu-id="1bb37-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1bb37-119">Name</span></span>|<span data-ttu-id="1bb37-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1bb37-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1bb37-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bb37-121">Authorization</span></span>|<span data-ttu-id="1bb37-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bb37-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb37-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bb37-124">Request body</span></span>

<span data-ttu-id="1bb37-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bb37-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bb37-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bb37-126">Response</span></span>

<span data-ttu-id="1bb37-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1bb37-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1bb37-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bb37-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1bb37-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bb37-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1bb37-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb37-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="1bb37-131">C#</span><span class="sxs-lookup"><span data-stu-id="1bb37-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bb37-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bb37-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bb37-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bb37-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bb37-134">Java</span><span class="sxs-lookup"><span data-stu-id="1bb37-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1bb37-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bb37-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
