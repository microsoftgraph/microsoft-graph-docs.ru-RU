---
title: 'раздел: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: cf621b42f958eaae5317084cac90abde1e2a8069
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336115"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="0e163-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="0e163-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e163-104">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="0e163-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="0e163-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="0e163-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e163-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e163-106">Permissions</span></span>
<span data-ttu-id="0e163-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e163-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e163-109">Permission type</span></span>      | <span data-ttu-id="0e163-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e163-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e163-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e163-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e163-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e163-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e163-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e163-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e163-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e163-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0e163-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e163-115">Application</span></span> | <span data-ttu-id="0e163-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e163-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e163-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e163-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="0e163-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e163-118">Request headers</span></span>
| <span data-ttu-id="0e163-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0e163-119">Name</span></span>       | <span data-ttu-id="0e163-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0e163-120">Type</span></span> | <span data-ttu-id="0e163-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0e163-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e163-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e163-122">Authorization</span></span>  | <span data-ttu-id="0e163-123">строка</span><span class="sxs-lookup"><span data-stu-id="0e163-123">string</span></span>  | <span data-ttu-id="0e163-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e163-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e163-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e163-126">Content-Type</span></span> | <span data-ttu-id="0e163-127">string</span><span class="sxs-lookup"><span data-stu-id="0e163-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0e163-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e163-128">Request body</span></span>
<span data-ttu-id="0e163-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="0e163-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="0e163-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="0e163-130">Parameter</span></span>    | <span data-ttu-id="0e163-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e163-131">Type</span></span>   |<span data-ttu-id="0e163-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e163-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e163-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="0e163-133">siteCollectionId</span></span>|<span data-ttu-id="0e163-134">String</span><span class="sxs-lookup"><span data-stu-id="0e163-134">String</span></span>|<span data-ttu-id="0e163-135">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="0e163-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="0e163-136">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e163-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="0e163-137">siteId</span><span class="sxs-lookup"><span data-stu-id="0e163-137">siteId</span></span>|<span data-ttu-id="0e163-138">String</span><span class="sxs-lookup"><span data-stu-id="0e163-138">String</span></span>|<span data-ttu-id="0e163-139">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="0e163-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="0e163-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e163-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="0e163-141">groupId</span><span class="sxs-lookup"><span data-stu-id="0e163-141">groupId</span></span>|<span data-ttu-id="0e163-142">String</span><span class="sxs-lookup"><span data-stu-id="0e163-142">String</span></span>|<span data-ttu-id="0e163-143">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="0e163-143">The id of the group to copy to.</span></span> <span data-ttu-id="0e163-144">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e163-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="0e163-145">id</span><span class="sxs-lookup"><span data-stu-id="0e163-145">id</span></span>|<span data-ttu-id="0e163-146">String</span><span class="sxs-lookup"><span data-stu-id="0e163-146">String</span></span>|<span data-ttu-id="0e163-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e163-147">Required.</span></span> <span data-ttu-id="0e163-148">Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="0e163-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="0e163-149">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="0e163-149">renameAs</span></span>|<span data-ttu-id="0e163-150">String</span><span class="sxs-lookup"><span data-stu-id="0e163-150">String</span></span>|<span data-ttu-id="0e163-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="0e163-151">The name of the copy.</span></span> <span data-ttu-id="0e163-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="0e163-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="0e163-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e163-153">Response</span></span>

<span data-ttu-id="0e163-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="0e163-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="0e163-155">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="0e163-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="0e163-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0e163-156">Example</span></span>
<span data-ttu-id="0e163-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e163-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e163-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e163-158">Request</span></span>
<span data-ttu-id="0e163-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e163-159">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0e163-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e163-160">Response</span></span>
<span data-ttu-id="0e163-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e163-161">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
