---
title: Обновление outlooktaskfolder
description: Обновление свойств, доступных для записи, папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5beff9ec781d03cd19f7dc147c4041b72f0f1b0f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265718"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="4d906-103">Обновление outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="4d906-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d906-104">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4d906-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="4d906-105">Вы не можете изменить значение свойства **Name** папки задач по умолчанию, "задачи".</span><span class="sxs-lookup"><span data-stu-id="4d906-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="4d906-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d906-106">Permissions</span></span>
<span data-ttu-id="4d906-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d906-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d906-109">Permission type</span></span>      | <span data-ttu-id="4d906-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d906-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d906-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d906-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d906-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d906-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4d906-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d906-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d906-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d906-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4d906-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d906-115">Application</span></span> | <span data-ttu-id="4d906-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d906-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d906-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d906-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4d906-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d906-118">Optional request headers</span></span>
| <span data-ttu-id="4d906-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4d906-119">Name</span></span>       | <span data-ttu-id="4d906-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4d906-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4d906-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d906-121">Authorization</span></span>  | <span data-ttu-id="4d906-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d906-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d906-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d906-124">Request body</span></span>
<span data-ttu-id="4d906-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4d906-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4d906-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d906-128">Property</span></span>     | <span data-ttu-id="4d906-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4d906-129">Type</span></span>   |<span data-ttu-id="4d906-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4d906-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d906-131">name</span><span class="sxs-lookup"><span data-stu-id="4d906-131">name</span></span>|<span data-ttu-id="4d906-132">String</span><span class="sxs-lookup"><span data-stu-id="4d906-132">String</span></span>|<span data-ttu-id="4d906-133">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="4d906-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="4d906-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d906-134">Response</span></span>

<span data-ttu-id="4d906-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d906-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d906-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4d906-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d906-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d906-137">Request</span></span>
<span data-ttu-id="4d906-138">В следующем примере показано изменение имени указанной папки задач на `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="4d906-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="4d906-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d906-139">Response</span></span>
<span data-ttu-id="4d906-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d906-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d906-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4d906-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d906-144">C#</span><span class="sxs-lookup"><span data-stu-id="4d906-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktaskfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d906-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d906-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktaskfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4d906-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4d906-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlooktaskfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
