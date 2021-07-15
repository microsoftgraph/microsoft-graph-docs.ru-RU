---
title: Удаление tenantTag
description: Удаляет объект tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 6bfecf4ff74b3e942536a07ca3dda129b44e86b3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441187"
---
# <a name="delete-tenanttag"></a><span data-ttu-id="84dea-103">Удаление tenantTag</span><span class="sxs-lookup"><span data-stu-id="84dea-103">Delete tenantTag</span></span>
<span data-ttu-id="84dea-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="84dea-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84dea-105">Удаляет объект [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="84dea-105">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84dea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84dea-106">Permissions</span></span>
<span data-ttu-id="84dea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84dea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84dea-109">Permission type</span></span>|<span data-ttu-id="84dea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84dea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84dea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84dea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84dea-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="84dea-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="84dea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84dea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84dea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84dea-114">Not supported.</span></span>|
|<span data-ttu-id="84dea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84dea-115">Application</span></span>|<span data-ttu-id="84dea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84dea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84dea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84dea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="84dea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84dea-118">Request headers</span></span>
|<span data-ttu-id="84dea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="84dea-119">Name</span></span>|<span data-ttu-id="84dea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="84dea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84dea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84dea-121">Authorization</span></span>|<span data-ttu-id="84dea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84dea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84dea-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84dea-124">Request body</span></span>
<span data-ttu-id="84dea-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84dea-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84dea-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="84dea-126">Response</span></span>

<span data-ttu-id="84dea-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="84dea-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="84dea-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="84dea-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84dea-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="84dea-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="84dea-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="84dea-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tenanttag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```
# <a name="c"></a>[<span data-ttu-id="84dea-131">C#</span><span class="sxs-lookup"><span data-stu-id="84dea-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84dea-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84dea-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84dea-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84dea-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84dea-134">Java</span><span class="sxs-lookup"><span data-stu-id="84dea-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="84dea-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84dea-135">Response</span></span>
><span data-ttu-id="84dea-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84dea-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
