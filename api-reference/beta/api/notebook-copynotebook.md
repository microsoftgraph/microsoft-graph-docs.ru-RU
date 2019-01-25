---
title: 'notebook: copyNotebook'
description: Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7100d768fb411aeab8ccbd0622de26aeae8a7133
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515603"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="09514-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="09514-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09514-p102">Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="09514-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="09514-107">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="09514-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="09514-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09514-108">Permissions</span></span>
<span data-ttu-id="09514-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09514-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09514-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09514-111">Permission type</span></span>      | <span data-ttu-id="09514-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09514-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09514-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09514-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09514-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09514-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="09514-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09514-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09514-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09514-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="09514-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09514-117">Application</span></span> | <span data-ttu-id="09514-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09514-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09514-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09514-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="09514-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09514-120">Request headers</span></span>
| <span data-ttu-id="09514-121">Имя</span><span class="sxs-lookup"><span data-stu-id="09514-121">Name</span></span>       | <span data-ttu-id="09514-122">Тип</span><span class="sxs-lookup"><span data-stu-id="09514-122">Type</span></span> | <span data-ttu-id="09514-123">Описание</span><span class="sxs-lookup"><span data-stu-id="09514-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09514-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09514-124">Authorization</span></span>  | <span data-ttu-id="09514-125">строка</span><span class="sxs-lookup"><span data-stu-id="09514-125">string</span></span>  | <span data-ttu-id="09514-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09514-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09514-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09514-128">Content-Type</span></span> | <span data-ttu-id="09514-129">string</span><span class="sxs-lookup"><span data-stu-id="09514-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="09514-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09514-130">Request body</span></span>
<span data-ttu-id="09514-p105">В теле запроса укажите объект JSON, который содержит параметры, требуемые операцией. Если тело не нужно, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="09514-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="09514-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="09514-133">Parameter</span></span>    | <span data-ttu-id="09514-134">Тип</span><span class="sxs-lookup"><span data-stu-id="09514-134">Type</span></span>   |<span data-ttu-id="09514-135">Описание</span><span class="sxs-lookup"><span data-stu-id="09514-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09514-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="09514-136">siteCollectionId</span></span>|<span data-ttu-id="09514-137">String</span><span class="sxs-lookup"><span data-stu-id="09514-137">String</span></span>|<span data-ttu-id="09514-138">Идентификатор сайта SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="09514-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="09514-139">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="09514-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="09514-140">siteId</span><span class="sxs-lookup"><span data-stu-id="09514-140">siteId</span></span>|<span data-ttu-id="09514-141">String</span><span class="sxs-lookup"><span data-stu-id="09514-141">String</span></span>|<span data-ttu-id="09514-142">Идентификатор веб-сайта SharePoint, чтобы скопировать.</span><span class="sxs-lookup"><span data-stu-id="09514-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="09514-143">Используйте только при копировании на сайте группы разработчиков Office 365.</span><span class="sxs-lookup"><span data-stu-id="09514-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="09514-144">groupId</span><span class="sxs-lookup"><span data-stu-id="09514-144">groupId</span></span>|<span data-ttu-id="09514-145">String</span><span class="sxs-lookup"><span data-stu-id="09514-145">String</span></span>|<span data-ttu-id="09514-p108">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="09514-p108">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="09514-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="09514-148">renameAs</span></span>|<span data-ttu-id="09514-149">String</span><span class="sxs-lookup"><span data-stu-id="09514-149">String</span></span>|<span data-ttu-id="09514-p109">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="09514-p109">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="09514-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="09514-152">Response</span></span>

<span data-ttu-id="09514-p110">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="09514-p110">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="09514-155">Пример</span><span class="sxs-lookup"><span data-stu-id="09514-155">Example</span></span>
<span data-ttu-id="09514-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="09514-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09514-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="09514-157">Request</span></span>
<span data-ttu-id="09514-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09514-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="09514-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="09514-159">Response</span></span>
<span data-ttu-id="09514-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09514-160">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
