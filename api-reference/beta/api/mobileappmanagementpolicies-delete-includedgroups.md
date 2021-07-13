---
title: Delete includedGroup
description: Удаление группы из списка групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 00f49c6c0ccb34fd18de68b65fc9f6ce7ff94605
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401367"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="0c446-103">Delete includedGroup</span><span class="sxs-lookup"><span data-stu-id="0c446-103">Delete includedGroup</span></span>

<span data-ttu-id="0c446-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c446-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c446-105">Удаление группы из списка групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="0c446-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c446-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c446-106">Permissions</span></span>

<span data-ttu-id="0c446-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c446-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c446-109">Permission type</span></span>|<span data-ttu-id="0c446-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c446-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c446-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c446-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c446-112">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="0c446-112">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="0c446-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c446-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c446-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c446-114">Not supported.</span></span>|
|<span data-ttu-id="0c446-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c446-115">Application</span></span> | <span data-ttu-id="0c446-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c446-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c446-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c446-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0c446-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c446-118">Request headers</span></span>

|<span data-ttu-id="0c446-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c446-119">Name</span></span>|<span data-ttu-id="0c446-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c446-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c446-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c446-121">Authorization</span></span>|<span data-ttu-id="0c446-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c446-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c446-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c446-124">Request body</span></span>

<span data-ttu-id="0c446-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c446-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c446-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c446-126">Response</span></span>

<span data-ttu-id="0c446-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c446-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c446-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c446-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c446-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c446-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0c446-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c446-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```
# <a name="c"></a>[<span data-ttu-id="0c446-132">C#</span><span class="sxs-lookup"><span data-stu-id="0c446-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c446-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c446-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c446-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c446-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c446-135">Java</span><span class="sxs-lookup"><span data-stu-id="0c446-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c446-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c446-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
