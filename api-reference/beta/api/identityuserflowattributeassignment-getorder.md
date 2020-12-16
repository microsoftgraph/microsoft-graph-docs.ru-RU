---
title: 'identityUserFlowAttributeAssignment: getOrder'
description: Получите порядок identityUserFlowAttributeAssignments, собираемого в пользовательском потоке.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 19172e8928716cb3f7ad49e67bc2f75de122de46
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689266"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="3a466-103">identityUserFlowAttributeAssignment: getOrder</span><span class="sxs-lookup"><span data-stu-id="3a466-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="3a466-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a466-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a466-105">Получите порядок identityUserFlowAttributeAssignments, собираемого в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="3a466-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a466-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a466-106">Permissions</span></span>

<span data-ttu-id="3a466-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a466-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a466-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a466-109">Permission type</span></span>|<span data-ttu-id="3a466-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a466-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a466-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a466-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a466-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a466-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3a466-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a466-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a466-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a466-114">Not supported</span></span>|
|<span data-ttu-id="3a466-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a466-115">Application</span></span>|<span data-ttu-id="3a466-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a466-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a466-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a466-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="3a466-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a466-118">Request headers</span></span>

|<span data-ttu-id="3a466-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3a466-119">Name</span></span>|<span data-ttu-id="3a466-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a466-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a466-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a466-121">Authorization</span></span>|<span data-ttu-id="3a466-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a466-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="3a466-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3a466-124">Function parameters</span></span>

<span data-ttu-id="3a466-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a466-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a466-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a466-126">Response</span></span>

<span data-ttu-id="3a466-127">В случае успешного выполнения эта функция возвращает код `200 OK` отклика и [assignmentOrder](../resources/assignmentorder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a466-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a466-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a466-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a466-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a466-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3a466-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a466-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```
# <a name="c"></a>[<span data-ttu-id="3a466-131">C#</span><span class="sxs-lookup"><span data-stu-id="3a466-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-getorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a466-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a466-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-getorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a466-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a466-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-getorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a466-134">Java</span><span class="sxs-lookup"><span data-stu-id="3a466-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-getorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a466-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a466-135">Response</span></span>

<span data-ttu-id="3a466-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a466-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
