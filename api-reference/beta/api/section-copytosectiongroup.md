---
title: 'section: copyToSectionGroup'
description: Копирование раздела в указанную группу разделов.
localization_priority: Normal
ms.openlocfilehash: 58907c479096843cdde82ab27eeb318a00fcd32f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858683"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="b99a4-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b99a4-103">section: copyToSectionGroup</span></span>

> <span data-ttu-id="b99a4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b99a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b99a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b99a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b99a4-106">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="b99a4-106">Copies a section to a specific section group.</span></span>

<span data-ttu-id="b99a4-107">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="b99a4-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b99a4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b99a4-108">Permissions</span></span>
<span data-ttu-id="b99a4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b99a4-111">Permission type</span></span>      | <span data-ttu-id="b99a4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b99a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b99a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b99a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b99a4-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99a4-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b99a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b99a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99a4-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b99a4-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b99a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b99a4-117">Application</span></span> | <span data-ttu-id="b99a4-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99a4-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b99a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b99a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="b99a4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b99a4-120">Request headers</span></span>
| <span data-ttu-id="b99a4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b99a4-121">Name</span></span>       | <span data-ttu-id="b99a4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b99a4-122">Type</span></span> | <span data-ttu-id="b99a4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b99a4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b99a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99a4-124">Authorization</span></span>  | <span data-ttu-id="b99a4-125">string</span><span class="sxs-lookup"><span data-stu-id="b99a4-125">string</span></span>  | <span data-ttu-id="b99a4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b99a4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b99a4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b99a4-128">Content-Type</span></span> | <span data-ttu-id="b99a4-129">string</span><span class="sxs-lookup"><span data-stu-id="b99a4-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b99a4-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b99a4-130">Request body</span></span>
<span data-ttu-id="b99a4-131">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="b99a4-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b99a4-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="b99a4-132">Parameter</span></span>    | <span data-ttu-id="b99a4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b99a4-133">Type</span></span>   |<span data-ttu-id="b99a4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b99a4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b99a4-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="b99a4-135">siteCollectionId</span></span>|<span data-ttu-id="b99a4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b99a4-136">String</span></span>|<span data-ttu-id="b99a4-137">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="b99a4-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="b99a4-138">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="b99a4-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b99a4-139">siteId</span><span class="sxs-lookup"><span data-stu-id="b99a4-139">siteId</span></span>|<span data-ttu-id="b99a4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b99a4-140">String</span></span>|<span data-ttu-id="b99a4-141">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="b99a4-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="b99a4-142">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="b99a4-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b99a4-143">groupId</span><span class="sxs-lookup"><span data-stu-id="b99a4-143">groupId</span></span>|<span data-ttu-id="b99a4-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b99a4-144">String</span></span>|<span data-ttu-id="b99a4-p106">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="b99a4-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b99a4-147">id</span><span class="sxs-lookup"><span data-stu-id="b99a4-147">id</span></span>|<span data-ttu-id="b99a4-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b99a4-148">String</span></span>|<span data-ttu-id="b99a4-p107">Обязательный. Идентификатор целевой группы разделов.</span><span class="sxs-lookup"><span data-stu-id="b99a4-p107">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="b99a4-151">renameAs</span><span class="sxs-lookup"><span data-stu-id="b99a4-151">renameAs</span></span>|<span data-ttu-id="b99a4-152">Строка</span><span class="sxs-lookup"><span data-stu-id="b99a4-152">String</span></span>|<span data-ttu-id="b99a4-p108">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="b99a4-p108">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="b99a4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b99a4-155">Response</span></span>

<span data-ttu-id="b99a4-p109">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="b99a4-p109">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b99a4-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b99a4-158">Example</span></span>
<span data-ttu-id="b99a4-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b99a4-159">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b99a4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b99a4-160">Request</span></span>
<span data-ttu-id="b99a4-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b99a4-161">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b99a4-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="b99a4-162">Response</span></span>
<span data-ttu-id="b99a4-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b99a4-163">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
