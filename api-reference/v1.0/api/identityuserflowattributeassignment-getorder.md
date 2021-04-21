---
title: 'identityUserFlowAttributeAssignment: getOrder'
description: Получите порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a3d513caab828c4b7704e8d7fd14be213e159db4
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920682"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="06606-103">identityUserFlowAttributeAssignment: getOrder</span><span class="sxs-lookup"><span data-stu-id="06606-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="06606-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06606-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06606-105">Получите порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="06606-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="06606-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06606-106">Permissions</span></span>

<span data-ttu-id="06606-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06606-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06606-109">Permission type</span></span>|<span data-ttu-id="06606-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06606-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06606-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06606-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06606-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06606-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="06606-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06606-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06606-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="06606-114">Not supported</span></span>|
|<span data-ttu-id="06606-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06606-115">Application</span></span>|<span data-ttu-id="06606-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06606-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06606-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06606-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="06606-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06606-118">Request headers</span></span>

|<span data-ttu-id="06606-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06606-119">Name</span></span>|<span data-ttu-id="06606-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06606-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06606-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06606-121">Authorization</span></span>|<span data-ttu-id="06606-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06606-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="06606-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="06606-124">Function parameters</span></span>

<span data-ttu-id="06606-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06606-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06606-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="06606-126">Response</span></span>

<span data-ttu-id="06606-127">В случае успешного выполнения данной функции возвращается код ответа и `200 OK` [назначениеOrder](../resources/assignmentorder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06606-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06606-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="06606-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06606-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="06606-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="06606-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="06606-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/getOrder
```
# <a name="c"></a>[<span data-ttu-id="06606-131">C#</span><span class="sxs-lookup"><span data-stu-id="06606-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-getorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06606-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06606-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-getorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06606-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06606-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-getorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06606-134">Java</span><span class="sxs-lookup"><span data-stu-id="06606-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-getorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06606-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="06606-135">Response</span></span>

<span data-ttu-id="06606-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06606-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta$metadata#microsoft.graph.assignmentOrder",
    "order": [
        "extension_GUID_ShoeSize",
        "City"
    ]
}
```
