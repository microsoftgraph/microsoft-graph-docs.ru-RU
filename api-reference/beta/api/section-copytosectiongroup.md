---
title: 'section: copyToSectionGroup'
description: Копирование раздела в указанную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 0b67f140871b6fa81c81f3e5ffceee492b62b3af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514168"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="b91c6-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b91c6-103">section: copyToSectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b91c6-104">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="b91c6-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="b91c6-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="b91c6-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b91c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b91c6-106">Permissions</span></span>
<span data-ttu-id="b91c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b91c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b91c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b91c6-109">Permission type</span></span>      | <span data-ttu-id="b91c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b91c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b91c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b91c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b91c6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b91c6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b91c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b91c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b91c6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b91c6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b91c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b91c6-115">Application</span></span> | <span data-ttu-id="b91c6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b91c6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b91c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b91c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="b91c6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b91c6-118">Request headers</span></span>
| <span data-ttu-id="b91c6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b91c6-119">Name</span></span>       | <span data-ttu-id="b91c6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b91c6-120">Type</span></span> | <span data-ttu-id="b91c6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b91c6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b91c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b91c6-122">Authorization</span></span>  | <span data-ttu-id="b91c6-123">строка</span><span class="sxs-lookup"><span data-stu-id="b91c6-123">string</span></span>  | <span data-ttu-id="b91c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b91c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b91c6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b91c6-126">Content-Type</span></span> | <span data-ttu-id="b91c6-127">string</span><span class="sxs-lookup"><span data-stu-id="b91c6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b91c6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b91c6-128">Request body</span></span>
<span data-ttu-id="b91c6-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="b91c6-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b91c6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="b91c6-130">Parameter</span></span>    | <span data-ttu-id="b91c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b91c6-131">Type</span></span>   |<span data-ttu-id="b91c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b91c6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b91c6-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="b91c6-133">siteCollectionId</span></span>|<span data-ttu-id="b91c6-134">String</span><span class="sxs-lookup"><span data-stu-id="b91c6-134">String</span></span>|<span data-ttu-id="b91c6-135">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="b91c6-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="b91c6-136">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="b91c6-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b91c6-137">siteId</span><span class="sxs-lookup"><span data-stu-id="b91c6-137">siteId</span></span>|<span data-ttu-id="b91c6-138">String</span><span class="sxs-lookup"><span data-stu-id="b91c6-138">String</span></span>|<span data-ttu-id="b91c6-139">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="b91c6-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="b91c6-140">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="b91c6-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b91c6-141">groupId</span><span class="sxs-lookup"><span data-stu-id="b91c6-141">groupId</span></span>|<span data-ttu-id="b91c6-142">String</span><span class="sxs-lookup"><span data-stu-id="b91c6-142">String</span></span>|<span data-ttu-id="b91c6-p105">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="b91c6-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b91c6-145">id</span><span class="sxs-lookup"><span data-stu-id="b91c6-145">id</span></span>|<span data-ttu-id="b91c6-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b91c6-146">String</span></span>|<span data-ttu-id="b91c6-p106">Обязательный. Идентификатор целевой группы разделов.</span><span class="sxs-lookup"><span data-stu-id="b91c6-p106">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="b91c6-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="b91c6-149">renameAs</span></span>|<span data-ttu-id="b91c6-150">String</span><span class="sxs-lookup"><span data-stu-id="b91c6-150">String</span></span>|<span data-ttu-id="b91c6-p107">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="b91c6-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="b91c6-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b91c6-153">Response</span></span>

<span data-ttu-id="b91c6-p108">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="b91c6-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b91c6-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b91c6-156">Example</span></span>
<span data-ttu-id="b91c6-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b91c6-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b91c6-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b91c6-158">Request</span></span>
<span data-ttu-id="b91c6-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b91c6-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="b91c6-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="b91c6-160">Response</span></span>
<span data-ttu-id="b91c6-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b91c6-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytosectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
