---
title: 'educationSubmission: setUpResourcesFolder'
description: Запуск создания папки SharePoint, в которой все ресурсы на основе файлов (Word, Excel и так далее) должны быть загружены для данной отправки.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c4acc92ad0c95041b39e84f04849d2f4095eab50
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870138"
---
# <a name="educationsubmission-setupresourcesfolder"></a><span data-ttu-id="24600-103">educationSubmission: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="24600-103">educationSubmission: setUpResourcesFolder</span></span>

<span data-ttu-id="24600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24600-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24600-105">Запуск создания папки SharePoint, в которой все ресурсы на основе файлов (Word, Excel и так далее) должны быть загружены для данной отправки.</span><span class="sxs-lookup"><span data-stu-id="24600-105">Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission.</span></span>

<span data-ttu-id="24600-106">Обратите внимание, что файлы должны быть размещены в этой папке, чтобы они были добавлены в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="24600-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="24600-107">Только учащийся в классе может определить, какие файлы загрузить в данной папке ресурсов на уровне отправки.</span><span class="sxs-lookup"><span data-stu-id="24600-107">Only a student in the class can determine what files to upload in a given submission-level resource folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="24600-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24600-108">Permissions</span></span>
<span data-ttu-id="24600-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24600-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24600-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24600-111">Permission type</span></span>      | <span data-ttu-id="24600-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24600-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24600-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24600-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="24600-114">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="24600-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="24600-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24600-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="24600-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24600-116">Not supported.</span></span>  |
|<span data-ttu-id="24600-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24600-117">Application</span></span> | <span data-ttu-id="24600-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24600-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="24600-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24600-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/setUpResourcesFolder
```

## <a name="request-headers"></a><span data-ttu-id="24600-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24600-120">Request headers</span></span>
| <span data-ttu-id="24600-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24600-121">Header</span></span>       | <span data-ttu-id="24600-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24600-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24600-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24600-123">Authorization</span></span>  | <span data-ttu-id="24600-p103">Bearer `{token}`. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="24600-p103">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24600-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24600-126">Request body</span></span>
<span data-ttu-id="24600-127">Предоставление пустого json `{}` в качестве тела запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24600-127">Provide an empty json `{}` as request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24600-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="24600-128">Response</span></span>
<span data-ttu-id="24600-129">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="24600-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="24600-130">Тело будет содержать модель отправки.</span><span class="sxs-lookup"><span data-stu-id="24600-130">The body will contain the submission model.</span></span>

## <a name="example"></a><span data-ttu-id="24600-131">Пример</span><span class="sxs-lookup"><span data-stu-id="24600-131">Example</span></span>
<span data-ttu-id="24600-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="24600-132">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="24600-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24600-133">Request</span></span>
<span data-ttu-id="24600-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24600-134">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="24600-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="24600-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/submissions/20302/setUpResourcesFolder
Content-type: application/json

{
}
```
# <a name="c"></a>[<span data-ttu-id="24600-136">C#</span><span class="sxs-lookup"><span data-stu-id="24600-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24600-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24600-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24600-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24600-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24600-139">Java</span><span class="sxs-lookup"><span data-stu-id="24600-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="24600-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="24600-140">Response</span></span>
<span data-ttu-id="24600-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24600-141">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions/$entity",
    "status": "working",
    "submittedDateTime": null,
    "unsubmittedDateTime": null,
    "returnedDateTime": null,
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
    "id": "803fb5dd-3553-455f-3d94-f79fb54a1003",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "resources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/resources",
    "resources": [],
    "submittedResources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/submittedResources",
    "submittedResources": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-d4113fc72dc1
2021-05-12 12:00:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: setUpResourcesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


