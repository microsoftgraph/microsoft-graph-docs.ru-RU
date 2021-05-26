---
title: Сброс синхронизации на educationSynchronizationProfile
description: Сброс синхронизации определенного профиля синхронизации школьных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 51a41991726ec9349f7f3f702973c8040031c39b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664736"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="cfef4-103">Сброс синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="cfef4-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="cfef4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfef4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfef4-105">Сброс синхронизации определенного профиля синхронизации [школьных](../resources/educationsynchronizationprofile.md) данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="cfef4-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="cfef4-106">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cfef4-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="cfef4-107">Все ошибки, с которыми столкнулись, будут удалены.</span><span class="sxs-lookup"><span data-stu-id="cfef4-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="cfef4-108">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cfef4-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="cfef4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfef4-109">Permissions</span></span>
<span data-ttu-id="cfef4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfef4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfef4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfef4-112">Permission type</span></span> | <span data-ttu-id="cfef4-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfef4-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cfef4-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfef4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cfef4-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfef4-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="cfef4-116">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfef4-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cfef4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfef4-117">Not supported.</span></span>|
|<span data-ttu-id="cfef4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="cfef4-118">Application</span></span>|<span data-ttu-id="cfef4-119">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfef4-119">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfef4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfef4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="cfef4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfef4-121">Request headers</span></span>
| <span data-ttu-id="cfef4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cfef4-122">Name</span></span>       | <span data-ttu-id="cfef4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cfef4-123">Type</span></span> | <span data-ttu-id="cfef4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cfef4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cfef4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfef4-125">Authorization</span></span>  | <span data-ttu-id="cfef4-126">string</span><span class="sxs-lookup"><span data-stu-id="cfef4-126">string</span></span>  | <span data-ttu-id="cfef4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfef4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfef4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfef4-129">Request body</span></span>
<span data-ttu-id="cfef4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfef4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cfef4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfef4-131">Response</span></span>
<span data-ttu-id="cfef4-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="cfef4-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cfef4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cfef4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfef4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfef4-134">Request</span></span>
<span data-ttu-id="cfef4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfef4-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfef4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfef4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="cfef4-137">C#</span><span class="sxs-lookup"><span data-stu-id="cfef4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfef4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfef4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfef4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfef4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfef4-140">Java</span><span class="sxs-lookup"><span data-stu-id="cfef4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfef4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfef4-141">Response</span></span>

<span data-ttu-id="cfef4-142">Тело ответа не существует.</span><span class="sxs-lookup"><span data-stu-id="cfef4-142">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


