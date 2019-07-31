---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6ae3c6663621edcdeb08839c645a9cd0f7ae6e81
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954839"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="3fa3e-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="3fa3e-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa3e-104">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="3fa3e-105">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="3fa3e-106">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="3fa3e-107">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3fa3e-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="3fa3e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa3e-108">Permissions</span></span>
<span data-ttu-id="3fa3e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fa3e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa3e-111">Permission type</span></span> | <span data-ttu-id="3fa3e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa3e-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3fa3e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa3e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3fa3e-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fa3e-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3fa3e-115">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa3e-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3fa3e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-116">Not supported.</span></span>|
|<span data-ttu-id="3fa3e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fa3e-117">Application</span></span>|<span data-ttu-id="3fa3e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa3e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa3e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="3fa3e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa3e-120">Request headers</span></span>
| <span data-ttu-id="3fa3e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3fa3e-121">Name</span></span>       | <span data-ttu-id="3fa3e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3fa3e-122">Type</span></span> | <span data-ttu-id="3fa3e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa3e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3fa3e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa3e-124">Authorization</span></span>  | <span data-ttu-id="3fa3e-125">string</span><span class="sxs-lookup"><span data-stu-id="3fa3e-125">string</span></span>  | <span data-ttu-id="3fa3e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fa3e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fa3e-128">Request body</span></span>
<span data-ttu-id="3fa3e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3fa3e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa3e-130">Response</span></span>
<span data-ttu-id="3fa3e-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3fa3e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa3e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fa3e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa3e-133">Request</span></span>
<span data-ttu-id="3fa3e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3fa3e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa3e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3fa3e-136">C#</span><span class="sxs-lookup"><span data-stu-id="3fa3e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3fa3e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3fa3e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3fa3e-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3fa3e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3fa3e-139">Java</span><span class="sxs-lookup"><span data-stu-id="3fa3e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3fa3e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa3e-140">Response</span></span>

<span data-ttu-id="3fa3e-141">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="3fa3e-141">There is no response body.</span></span>

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
