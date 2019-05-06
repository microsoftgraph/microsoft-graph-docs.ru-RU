---
title: Обновление outlooktaskgroup
description: Обновление свойств, доступных для записи, для группы задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d617ecc2cdad3c6c720cf8800161761a565ae173
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596163"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="90db9-103">Обновление outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="90db9-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90db9-104">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="90db9-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="90db9-105">Обратите внимание, что нельзя изменить имя группы задач по умолчанию "Мои задачи".</span><span class="sxs-lookup"><span data-stu-id="90db9-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="90db9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90db9-106">Permissions</span></span>
<span data-ttu-id="90db9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90db9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90db9-109">Permission type</span></span>      | <span data-ttu-id="90db9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90db9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90db9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90db9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90db9-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90db9-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="90db9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90db9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90db9-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90db9-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="90db9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90db9-115">Application</span></span> | <span data-ttu-id="90db9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90db9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90db9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90db9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="90db9-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90db9-118">Optional request headers</span></span>
| <span data-ttu-id="90db9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90db9-119">Name</span></span>       | <span data-ttu-id="90db9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90db9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="90db9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90db9-121">Authorization</span></span>  | <span data-ttu-id="90db9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90db9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90db9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90db9-124">Request body</span></span>
<span data-ttu-id="90db9-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="90db9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="90db9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="90db9-128">Property</span></span>     | <span data-ttu-id="90db9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="90db9-129">Type</span></span>   |<span data-ttu-id="90db9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="90db9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90db9-131">name</span><span class="sxs-lookup"><span data-stu-id="90db9-131">name</span></span>|<span data-ttu-id="90db9-132">String</span><span class="sxs-lookup"><span data-stu-id="90db9-132">String</span></span>|<span data-ttu-id="90db9-133">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="90db9-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="90db9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90db9-134">Response</span></span>

<span data-ttu-id="90db9-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90db9-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90db9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="90db9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90db9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="90db9-137">Request</span></span>
<span data-ttu-id="90db9-138">В следующем примере имя группы задач изменяется на "личные задачи".</span><span class="sxs-lookup"><span data-stu-id="90db9-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
##### <a name="response"></a><span data-ttu-id="90db9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="90db9-139">Response</span></span>
<span data-ttu-id="90db9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90db9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="90db9-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="90db9-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="90db9-144">Языках</span><span class="sxs-lookup"><span data-stu-id="90db9-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90db9-145">Язык</span><span class="sxs-lookup"><span data-stu-id="90db9-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
