---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 254eab3b8ac40f7c477ceba68e529a4e1998a9b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424395"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="c26b3-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="c26b3-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="c26b3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c26b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c26b3-105">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c26b3-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="c26b3-106">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c26b3-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="c26b3-107">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="c26b3-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="c26b3-108">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c26b3-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c26b3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c26b3-109">Permissions</span></span>
<span data-ttu-id="c26b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c26b3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c26b3-112">Permission type</span></span> | <span data-ttu-id="c26b3-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c26b3-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c26b3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c26b3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c26b3-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c26b3-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c26b3-116">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c26b3-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c26b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c26b3-117">Not supported.</span></span>|
|<span data-ttu-id="c26b3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c26b3-118">Application</span></span>|<span data-ttu-id="c26b3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c26b3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c26b3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c26b3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="c26b3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c26b3-121">Request headers</span></span>
| <span data-ttu-id="c26b3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c26b3-122">Name</span></span>       | <span data-ttu-id="c26b3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c26b3-123">Type</span></span> | <span data-ttu-id="c26b3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c26b3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c26b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c26b3-125">Authorization</span></span>  | <span data-ttu-id="c26b3-126">string</span><span class="sxs-lookup"><span data-stu-id="c26b3-126">string</span></span>  | <span data-ttu-id="c26b3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c26b3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c26b3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c26b3-129">Request body</span></span>
<span data-ttu-id="c26b3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c26b3-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c26b3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c26b3-131">Response</span></span>
<span data-ttu-id="c26b3-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c26b3-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c26b3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c26b3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c26b3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c26b3-134">Request</span></span>
<span data-ttu-id="c26b3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c26b3-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c26b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c26b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="c26b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="c26b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c26b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c26b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c26b3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c26b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c26b3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c26b3-140">Response</span></span>

<span data-ttu-id="c26b3-141">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="c26b3-141">There is no response body.</span></span>

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
