---
title: 'identityUserFlowAttributeAssignment: getOrder'
description: Получите порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ea6e8aa4e5f27d0ae21b1ae593f045b29a5848af
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883067"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="32bc6-103">identityUserFlowAttributeAssignment: getOrder</span><span class="sxs-lookup"><span data-stu-id="32bc6-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="32bc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32bc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32bc6-105">Получите порядок сбора удостоверенийUserFlowAttributeAssignments в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="32bc6-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="32bc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32bc6-106">Permissions</span></span>

<span data-ttu-id="32bc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32bc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32bc6-109">Permission type</span></span>|<span data-ttu-id="32bc6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32bc6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32bc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32bc6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32bc6-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bc6-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="32bc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32bc6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32bc6-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="32bc6-114">Not supported</span></span>|
|<span data-ttu-id="32bc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32bc6-115">Application</span></span>|<span data-ttu-id="32bc6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bc6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32bc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32bc6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="32bc6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32bc6-118">Request headers</span></span>

|<span data-ttu-id="32bc6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="32bc6-119">Name</span></span>|<span data-ttu-id="32bc6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="32bc6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32bc6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32bc6-121">Authorization</span></span>|<span data-ttu-id="32bc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32bc6-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="32bc6-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="32bc6-124">Function parameters</span></span>

<span data-ttu-id="32bc6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32bc6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32bc6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bc6-126">Response</span></span>

<span data-ttu-id="32bc6-127">В случае успешного выполнения данной функции возвращается код ответа и `200 OK` [назначениеOrder](../resources/assignmentorder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="32bc6-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32bc6-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="32bc6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32bc6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="32bc6-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/getOrder
```

### <a name="response"></a><span data-ttu-id="32bc6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bc6-130">Response</span></span>

<span data-ttu-id="32bc6-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32bc6-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
