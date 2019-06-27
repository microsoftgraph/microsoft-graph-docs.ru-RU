---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b6bfa7caadcb6b393a22d19a73c56159492da739
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259523"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="833ae-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="833ae-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="833ae-104">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="833ae-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="833ae-105">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="833ae-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="833ae-106">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="833ae-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="833ae-107">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="833ae-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="833ae-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="833ae-108">Permissions</span></span>
<span data-ttu-id="833ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="833ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="833ae-111">Permission type</span></span> | <span data-ttu-id="833ae-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="833ae-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="833ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="833ae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="833ae-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="833ae-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="833ae-115">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="833ae-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="833ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833ae-116">Not supported.</span></span>|
|<span data-ttu-id="833ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="833ae-117">Application</span></span>|<span data-ttu-id="833ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="833ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="833ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="833ae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="833ae-120">Request headers</span></span>
| <span data-ttu-id="833ae-121">Имя</span><span class="sxs-lookup"><span data-stu-id="833ae-121">Name</span></span>       | <span data-ttu-id="833ae-122">Тип</span><span class="sxs-lookup"><span data-stu-id="833ae-122">Type</span></span> | <span data-ttu-id="833ae-123">Описание</span><span class="sxs-lookup"><span data-stu-id="833ae-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="833ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="833ae-124">Authorization</span></span>  | <span data-ttu-id="833ae-125">string</span><span class="sxs-lookup"><span data-stu-id="833ae-125">string</span></span>  | <span data-ttu-id="833ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="833ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="833ae-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="833ae-128">Request body</span></span>
<span data-ttu-id="833ae-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="833ae-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="833ae-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="833ae-130">Response</span></span>
<span data-ttu-id="833ae-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="833ae-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="833ae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="833ae-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="833ae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="833ae-133">Request</span></span>
<span data-ttu-id="833ae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="833ae-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="833ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="833ae-135">Response</span></span>

<span data-ttu-id="833ae-136">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="833ae-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="833ae-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="833ae-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="833ae-138">C#</span><span class="sxs-lookup"><span data-stu-id="833ae-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="833ae-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="833ae-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="833ae-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="833ae-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
