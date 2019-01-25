---
title: 'page: copyToSection'
description: Копирование страницы в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dd7abb016345195bd5a32e20a5623d6fca9fd6ff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516443"
---
# <a name="page-copytosection"></a><span data-ttu-id="dfbec-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="dfbec-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfbec-104">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="dfbec-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="dfbec-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="dfbec-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfbec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbec-106">Permissions</span></span>
<span data-ttu-id="dfbec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbec-109">Permission type</span></span>      | <span data-ttu-id="dfbec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfbec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfbec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfbec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dfbec-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbec-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfbec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfbec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfbec-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfbec-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dfbec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfbec-115">Application</span></span> | <span data-ttu-id="dfbec-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbec-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfbec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfbec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="dfbec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfbec-118">Request headers</span></span>
| <span data-ttu-id="dfbec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dfbec-119">Name</span></span>       | <span data-ttu-id="dfbec-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbec-120">Type</span></span> | <span data-ttu-id="dfbec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbec-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfbec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfbec-122">Authorization</span></span>  | <span data-ttu-id="dfbec-123">строка</span><span class="sxs-lookup"><span data-stu-id="dfbec-123">string</span></span>  | <span data-ttu-id="dfbec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfbec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfbec-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfbec-126">Content-Type</span></span> | <span data-ttu-id="dfbec-127">string</span><span class="sxs-lookup"><span data-stu-id="dfbec-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dfbec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfbec-128">Request body</span></span>
<span data-ttu-id="dfbec-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="dfbec-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="dfbec-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="dfbec-130">Parameter</span></span>    | <span data-ttu-id="dfbec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbec-131">Type</span></span>   |<span data-ttu-id="dfbec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfbec-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="dfbec-133">siteCollectionId</span></span>|<span data-ttu-id="dfbec-134">String</span><span class="sxs-lookup"><span data-stu-id="dfbec-134">String</span></span>|<span data-ttu-id="dfbec-135">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="dfbec-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="dfbec-136">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="dfbec-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dfbec-137">siteId</span><span class="sxs-lookup"><span data-stu-id="dfbec-137">siteId</span></span>|<span data-ttu-id="dfbec-138">String</span><span class="sxs-lookup"><span data-stu-id="dfbec-138">String</span></span>|<span data-ttu-id="dfbec-139">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="dfbec-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="dfbec-140">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="dfbec-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dfbec-141">groupId</span><span class="sxs-lookup"><span data-stu-id="dfbec-141">groupId</span></span>|<span data-ttu-id="dfbec-142">String</span><span class="sxs-lookup"><span data-stu-id="dfbec-142">String</span></span>|<span data-ttu-id="dfbec-p105">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="dfbec-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="dfbec-145">id</span><span class="sxs-lookup"><span data-stu-id="dfbec-145">id</span></span>|<span data-ttu-id="dfbec-146">String</span><span class="sxs-lookup"><span data-stu-id="dfbec-146">String</span></span>|<span data-ttu-id="dfbec-p106">Обязательный. Идентификатор целевого раздела.</span><span class="sxs-lookup"><span data-stu-id="dfbec-p106">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="dfbec-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfbec-149">Response</span></span>

<span data-ttu-id="dfbec-p107">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="dfbec-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="dfbec-152">Пример</span><span class="sxs-lookup"><span data-stu-id="dfbec-152">Example</span></span>
<span data-ttu-id="dfbec-153">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dfbec-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dfbec-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfbec-154">Request</span></span>
<span data-ttu-id="dfbec-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfbec-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="dfbec-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfbec-156">Response</span></span>
<span data-ttu-id="dfbec-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfbec-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
