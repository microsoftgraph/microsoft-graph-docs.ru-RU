---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 517dc5e2fddf0c959215fb69621e0bb99bad75e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965846"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="b1935-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="b1935-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="b1935-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1935-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1935-105">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b1935-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="b1935-106">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b1935-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="b1935-107">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="b1935-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="b1935-108">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b1935-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b1935-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1935-109">Permissions</span></span>
<span data-ttu-id="b1935-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1935-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1935-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1935-112">Permission type</span></span> | <span data-ttu-id="b1935-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1935-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b1935-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1935-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b1935-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1935-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b1935-116">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1935-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b1935-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1935-117">Not supported.</span></span>|
|<span data-ttu-id="b1935-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1935-118">Application</span></span>|<span data-ttu-id="b1935-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1935-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1935-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1935-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="b1935-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1935-121">Request headers</span></span>
| <span data-ttu-id="b1935-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b1935-122">Name</span></span>       | <span data-ttu-id="b1935-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b1935-123">Type</span></span> | <span data-ttu-id="b1935-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b1935-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1935-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1935-125">Authorization</span></span>  | <span data-ttu-id="b1935-126">string</span><span class="sxs-lookup"><span data-stu-id="b1935-126">string</span></span>  | <span data-ttu-id="b1935-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1935-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1935-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1935-129">Request body</span></span>
<span data-ttu-id="b1935-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1935-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b1935-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1935-131">Response</span></span>
<span data-ttu-id="b1935-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b1935-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1935-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b1935-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1935-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1935-134">Request</span></span>
<span data-ttu-id="b1935-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1935-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1935-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1935-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="b1935-137">C#</span><span class="sxs-lookup"><span data-stu-id="b1935-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1935-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1935-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1935-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1935-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1935-140">Java</span><span class="sxs-lookup"><span data-stu-id="b1935-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b1935-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1935-141">Response</span></span>

<span data-ttu-id="b1935-142">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="b1935-142">There is no response body.</span></span>

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


