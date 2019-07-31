---
title: Получение состояния Едукатионсинчронизатионпрофиле
description: Получение состояния определенного профиля синхронизации данных School в клиенте. Ответ будет указывать на состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1b9d8a1b8faf09ce9f70b4744dc116513b12c640
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954748"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="c52c4-104">Получение состояния Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="c52c4-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c52c4-105">Получение состояния определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c52c4-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c52c4-106">Ответ будет указывать на состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c52c4-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="c52c4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c52c4-107">Permissions</span></span>
<span data-ttu-id="c52c4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c52c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c52c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c52c4-110">Permission type</span></span> | <span data-ttu-id="c52c4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c52c4-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c52c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c52c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c52c4-113">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c52c4-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c52c4-114">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c52c4-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c52c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c52c4-115">Not supported.</span></span>|
|<span data-ttu-id="c52c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c52c4-116">Application</span></span>| <span data-ttu-id="c52c4-117">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c52c4-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c52c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c52c4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="c52c4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c52c4-119">Request headers</span></span>
| <span data-ttu-id="c52c4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c52c4-120">Name</span></span>       | <span data-ttu-id="c52c4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c52c4-121">Type</span></span> | <span data-ttu-id="c52c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c52c4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c52c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c52c4-123">Authorization</span></span>  | <span data-ttu-id="c52c4-124">string</span><span class="sxs-lookup"><span data-stu-id="c52c4-124">string</span></span>  | <span data-ttu-id="c52c4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c52c4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c52c4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c52c4-127">Request body</span></span>
<span data-ttu-id="c52c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c52c4-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c52c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c52c4-129">Response</span></span>
<span data-ttu-id="c52c4-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсинчронизатионпрофилестатус](../resources/educationsynchronizationprofilestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c52c4-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c52c4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c52c4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c52c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c52c4-132">Request</span></span>
<span data-ttu-id="c52c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c52c4-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c52c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c52c4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c52c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="c52c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c52c4-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c52c4-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c52c4-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c52c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c52c4-138">Java</span><span class="sxs-lookup"><span data-stu-id="c52c4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c52c4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c52c4-139">Response</span></span>
<span data-ttu-id="c52c4-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c52c4-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c52c4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c52c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
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
