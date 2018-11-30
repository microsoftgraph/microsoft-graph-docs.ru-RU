---
title: 'section: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
ms.openlocfilehash: 393618ddae4fa20b47bdb77aa650185f3b2ed518
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074606"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="2eb70-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="2eb70-103">section: copyToNotebook</span></span>

> <span data-ttu-id="2eb70-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2eb70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2eb70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2eb70-106">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="2eb70-106">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="2eb70-107">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="2eb70-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="2eb70-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2eb70-108">Permissions</span></span>
<span data-ttu-id="2eb70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2eb70-111">Permission type</span></span>      | <span data-ttu-id="2eb70-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2eb70-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2eb70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2eb70-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2eb70-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb70-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2eb70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2eb70-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eb70-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2eb70-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2eb70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2eb70-117">Application</span></span> | <span data-ttu-id="2eb70-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb70-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eb70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2eb70-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="2eb70-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2eb70-120">Request headers</span></span>
| <span data-ttu-id="2eb70-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2eb70-121">Name</span></span>       | <span data-ttu-id="2eb70-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb70-122">Type</span></span> | <span data-ttu-id="2eb70-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb70-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2eb70-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb70-124">Authorization</span></span>  | <span data-ttu-id="2eb70-125">string</span><span class="sxs-lookup"><span data-stu-id="2eb70-125">string</span></span>  | <span data-ttu-id="2eb70-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2eb70-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2eb70-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2eb70-128">Content-Type</span></span> | <span data-ttu-id="2eb70-129">string</span><span class="sxs-lookup"><span data-stu-id="2eb70-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2eb70-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2eb70-130">Request body</span></span>
<span data-ttu-id="2eb70-131">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="2eb70-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="2eb70-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="2eb70-132">Parameter</span></span>    | <span data-ttu-id="2eb70-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb70-133">Type</span></span>   |<span data-ttu-id="2eb70-134">Description</span><span class="sxs-lookup"><span data-stu-id="2eb70-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb70-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="2eb70-135">siteCollectionId</span></span>|<span data-ttu-id="2eb70-136">String</span><span class="sxs-lookup"><span data-stu-id="2eb70-136">String</span></span>|<span data-ttu-id="2eb70-137">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="2eb70-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="2eb70-138">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="2eb70-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2eb70-139">siteId</span><span class="sxs-lookup"><span data-stu-id="2eb70-139">siteId</span></span>|<span data-ttu-id="2eb70-140">String</span><span class="sxs-lookup"><span data-stu-id="2eb70-140">String</span></span>|<span data-ttu-id="2eb70-141">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="2eb70-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="2eb70-142">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="2eb70-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2eb70-143">groupId</span><span class="sxs-lookup"><span data-stu-id="2eb70-143">groupId</span></span>|<span data-ttu-id="2eb70-144">String</span><span class="sxs-lookup"><span data-stu-id="2eb70-144">String</span></span>|<span data-ttu-id="2eb70-p106">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="2eb70-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="2eb70-147">id</span><span class="sxs-lookup"><span data-stu-id="2eb70-147">id</span></span>|<span data-ttu-id="2eb70-148">Строка</span><span class="sxs-lookup"><span data-stu-id="2eb70-148">String</span></span>|<span data-ttu-id="2eb70-p107">Обязательный. Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="2eb70-p107">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="2eb70-151">renameAs</span><span class="sxs-lookup"><span data-stu-id="2eb70-151">renameAs</span></span>|<span data-ttu-id="2eb70-152">String</span><span class="sxs-lookup"><span data-stu-id="2eb70-152">String</span></span>|<span data-ttu-id="2eb70-p108">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="2eb70-p108">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="2eb70-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eb70-155">Response</span></span>

<span data-ttu-id="2eb70-p109">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="2eb70-p109">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="2eb70-158">Пример</span><span class="sxs-lookup"><span data-stu-id="2eb70-158">Example</span></span>
<span data-ttu-id="2eb70-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2eb70-159">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2eb70-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2eb70-160">Request</span></span>
<span data-ttu-id="2eb70-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2eb70-161">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2eb70-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="2eb70-162">Response</span></span>
<span data-ttu-id="2eb70-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2eb70-163">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->