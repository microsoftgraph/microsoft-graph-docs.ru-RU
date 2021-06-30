---
title: Delete includedGroup
description: Удаление группы из списка групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4097b71b17467f32d7b7c687c004ab4a8a59a556
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208339"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="79bea-103">Delete includedGroup</span><span class="sxs-lookup"><span data-stu-id="79bea-103">Delete includedGroup</span></span>

<span data-ttu-id="79bea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79bea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79bea-105">Удаление группы из списка групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="79bea-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="79bea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79bea-106">Permissions</span></span>

<span data-ttu-id="79bea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79bea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79bea-109">Permission type</span></span>|<span data-ttu-id="79bea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79bea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79bea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79bea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79bea-112">Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79bea-112">Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="79bea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79bea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79bea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79bea-114">Not supported.</span></span>|
|<span data-ttu-id="79bea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79bea-115">Application</span></span> | <span data-ttu-id="79bea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79bea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79bea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79bea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="79bea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79bea-118">Request headers</span></span>

|<span data-ttu-id="79bea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79bea-119">Name</span></span>|<span data-ttu-id="79bea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79bea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79bea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79bea-121">Authorization</span></span>|<span data-ttu-id="79bea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79bea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79bea-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79bea-124">Request body</span></span>

<span data-ttu-id="79bea-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79bea-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79bea-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="79bea-126">Response</span></span>

<span data-ttu-id="79bea-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="79bea-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79bea-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="79bea-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79bea-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="79bea-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="79bea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="79bea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```
# <a name="c"></a>[<span data-ttu-id="79bea-132">C#</span><span class="sxs-lookup"><span data-stu-id="79bea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79bea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79bea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79bea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79bea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79bea-135">Java</span><span class="sxs-lookup"><span data-stu-id="79bea-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79bea-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="79bea-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
