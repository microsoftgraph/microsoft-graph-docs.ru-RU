---
title: Получение состояния Едукатионсинчронизатионпрофиле
description: Получение состояния определенного профиля синхронизации данных School в клиенте. Ответ будет указывать на состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 30cde845220ecf2619516ddee1dcc5c58d3740c1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955345"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="6b182-104">Получение состояния Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="6b182-104">Get the status of an educationSynchronizationProfile</span></span>

<span data-ttu-id="6b182-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b182-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b182-106">Получение состояния определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6b182-106">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="6b182-107">Ответ будет указывать на состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6b182-107">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b182-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b182-108">Permissions</span></span>

<span data-ttu-id="6b182-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b182-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b182-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b182-111">Permission type</span></span>                       | <span data-ttu-id="6b182-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b182-112">Permissions (from least to most privileged)</span></span>                 |
| :------------------------------------ | :---------------------------------------------------------- |
| <span data-ttu-id="6b182-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b182-113">Delegated (work or school account)</span></span>    | <span data-ttu-id="6b182-114">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b182-114">EduAdministration.Read, EduAdministration.ReadWrite</span></span>         |
| <span data-ttu-id="6b182-115">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b182-115">Delegated (personal Microsoft account</span></span> | <span data-ttu-id="6b182-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b182-116">Not supported.</span></span>                                              |
| <span data-ttu-id="6b182-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b182-117">Application</span></span>                           | <span data-ttu-id="6b182-118">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6b182-118">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b182-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b182-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="6b182-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b182-120">Request headers</span></span>

| <span data-ttu-id="6b182-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6b182-121">Name</span></span>          | <span data-ttu-id="6b182-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6b182-122">Type</span></span>   | <span data-ttu-id="6b182-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6b182-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="6b182-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b182-124">Authorization</span></span> | <span data-ttu-id="6b182-125">string</span><span class="sxs-lookup"><span data-stu-id="6b182-125">string</span></span> | <span data-ttu-id="6b182-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b182-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b182-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b182-128">Request body</span></span>

<span data-ttu-id="6b182-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b182-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b182-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b182-130">Response</span></span>

<span data-ttu-id="6b182-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсинчронизатионпрофилестатус](../resources/educationsynchronizationprofilestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b182-131">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b182-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6b182-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6b182-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b182-133">Request</span></span>

<span data-ttu-id="6b182-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b182-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b182-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b182-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[<span data-ttu-id="6b182-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b182-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b182-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b182-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b182-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b182-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b182-139">Java</span><span class="sxs-lookup"><span data-stu-id="6b182-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b182-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b182-140">Response</span></span>

<span data-ttu-id="6b182-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b182-141">The following is an example of the response.</span></span>

> <span data-ttu-id="6b182-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b182-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
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


