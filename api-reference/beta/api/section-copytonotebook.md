---
title: 'section: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523325"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="ff79c-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="ff79c-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff79c-104">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="ff79c-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="ff79c-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="ff79c-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff79c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff79c-106">Permissions</span></span>
<span data-ttu-id="ff79c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff79c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff79c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff79c-109">Permission type</span></span>      | <span data-ttu-id="ff79c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff79c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff79c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff79c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff79c-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff79c-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff79c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff79c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff79c-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff79c-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ff79c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff79c-115">Application</span></span> | <span data-ttu-id="ff79c-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff79c-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff79c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff79c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="ff79c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff79c-118">Request headers</span></span>
| <span data-ttu-id="ff79c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ff79c-119">Name</span></span>       | <span data-ttu-id="ff79c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ff79c-120">Type</span></span> | <span data-ttu-id="ff79c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff79c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff79c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff79c-122">Authorization</span></span>  | <span data-ttu-id="ff79c-123">строка</span><span class="sxs-lookup"><span data-stu-id="ff79c-123">string</span></span>  | <span data-ttu-id="ff79c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff79c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff79c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff79c-126">Content-Type</span></span> | <span data-ttu-id="ff79c-127">string</span><span class="sxs-lookup"><span data-stu-id="ff79c-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ff79c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff79c-128">Request body</span></span>
<span data-ttu-id="ff79c-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="ff79c-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ff79c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ff79c-130">Parameter</span></span>    | <span data-ttu-id="ff79c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff79c-131">Type</span></span>   |<span data-ttu-id="ff79c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff79c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff79c-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="ff79c-133">siteCollectionId</span></span>|<span data-ttu-id="ff79c-134">String</span><span class="sxs-lookup"><span data-stu-id="ff79c-134">String</span></span>|<span data-ttu-id="ff79c-135">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="ff79c-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="ff79c-136">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="ff79c-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ff79c-137">siteId</span><span class="sxs-lookup"><span data-stu-id="ff79c-137">siteId</span></span>|<span data-ttu-id="ff79c-138">String</span><span class="sxs-lookup"><span data-stu-id="ff79c-138">String</span></span>|<span data-ttu-id="ff79c-139">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="ff79c-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="ff79c-140">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="ff79c-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ff79c-141">groupId</span><span class="sxs-lookup"><span data-stu-id="ff79c-141">groupId</span></span>|<span data-ttu-id="ff79c-142">String</span><span class="sxs-lookup"><span data-stu-id="ff79c-142">String</span></span>|<span data-ttu-id="ff79c-p105">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="ff79c-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ff79c-145">id</span><span class="sxs-lookup"><span data-stu-id="ff79c-145">id</span></span>|<span data-ttu-id="ff79c-146">String</span><span class="sxs-lookup"><span data-stu-id="ff79c-146">String</span></span>|<span data-ttu-id="ff79c-p106">Обязательный. Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ff79c-p106">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="ff79c-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="ff79c-149">renameAs</span></span>|<span data-ttu-id="ff79c-150">String</span><span class="sxs-lookup"><span data-stu-id="ff79c-150">String</span></span>|<span data-ttu-id="ff79c-p107">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="ff79c-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="ff79c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff79c-153">Response</span></span>

<span data-ttu-id="ff79c-p108">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="ff79c-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ff79c-156">Пример</span><span class="sxs-lookup"><span data-stu-id="ff79c-156">Example</span></span>
<span data-ttu-id="ff79c-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ff79c-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff79c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff79c-158">Request</span></span>
<span data-ttu-id="ff79c-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff79c-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="ff79c-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff79c-160">Response</span></span>
<span data-ttu-id="ff79c-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff79c-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytonotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
