---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f98548765e185d6bb3f66bbec33b50cd496c4804
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415983"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="d08d8-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="d08d8-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d08d8-104">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d08d8-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="d08d8-105">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d08d8-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="d08d8-106">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="d08d8-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="d08d8-107">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d08d8-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d08d8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d08d8-108">Permissions</span></span>
<span data-ttu-id="d08d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d08d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d08d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d08d8-111">Permission type</span></span> | <span data-ttu-id="d08d8-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d08d8-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d08d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d08d8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d08d8-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d08d8-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="d08d8-115">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d08d8-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d08d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d08d8-116">Not supported.</span></span>|
|<span data-ttu-id="d08d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d08d8-117">Application</span></span>|<span data-ttu-id="d08d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d08d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d08d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d08d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="d08d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d08d8-120">Request headers</span></span>
| <span data-ttu-id="d08d8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d08d8-121">Name</span></span>       | <span data-ttu-id="d08d8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d08d8-122">Type</span></span> | <span data-ttu-id="d08d8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d08d8-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d08d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d08d8-124">Authorization</span></span>  | <span data-ttu-id="d08d8-125">string</span><span class="sxs-lookup"><span data-stu-id="d08d8-125">string</span></span>  | <span data-ttu-id="d08d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d08d8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d08d8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d08d8-128">Request body</span></span>
<span data-ttu-id="d08d8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d08d8-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d08d8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d08d8-130">Response</span></span>
<span data-ttu-id="d08d8-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d08d8-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d08d8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d08d8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d08d8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d08d8-133">Request</span></span>
<span data-ttu-id="d08d8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d08d8-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d08d8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d08d8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d08d8-136">C#</span><span class="sxs-lookup"><span data-stu-id="d08d8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d08d8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d08d8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d08d8-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d08d8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d08d8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d08d8-139">Response</span></span>

<span data-ttu-id="d08d8-140">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="d08d8-140">There is no response body.</span></span>

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
