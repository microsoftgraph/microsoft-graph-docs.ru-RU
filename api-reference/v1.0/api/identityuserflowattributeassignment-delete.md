---
title: Удаление userAttributeAssignment
description: Удаление объекта identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2cf34a4e1da47a0c974585f430fa0d3f85dcf552
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883322"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="3ee75-103">Удаление userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3ee75-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="3ee75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ee75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ee75-105">Удаление [объекта identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ee75-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ee75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee75-106">Permissions</span></span>

<span data-ttu-id="3ee75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee75-109">Permission type</span></span>|<span data-ttu-id="3ee75-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ee75-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ee75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ee75-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ee75-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee75-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3ee75-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ee75-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ee75-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ee75-114">Not supported</span></span>|
|<span data-ttu-id="3ee75-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ee75-115">Application</span></span>|<span data-ttu-id="3ee75-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee75-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ee75-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ee75-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ee75-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ee75-118">Request headers</span></span>

|<span data-ttu-id="3ee75-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3ee75-119">Name</span></span>|<span data-ttu-id="3ee75-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3ee75-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ee75-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ee75-121">Authorization</span></span>|<span data-ttu-id="3ee75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ee75-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ee75-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ee75-124">Request body</span></span>

<span data-ttu-id="3ee75-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ee75-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee75-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ee75-126">Response</span></span>

<span data-ttu-id="3ee75-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3ee75-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3ee75-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ee75-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ee75-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ee75-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2xidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

### <a name="response"></a><span data-ttu-id="3ee75-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ee75-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
