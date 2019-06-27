---
title: Удаление Едукатионассигнментресаурце
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e38193b5b5185a6f602c517f0add386c758353f9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259908"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="cf162-103">Удаление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="cf162-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf162-104">Удаление ресурса из назначения.</span><span class="sxs-lookup"><span data-stu-id="cf162-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="cf162-105">Только преподаватели в классе могут удалить ресурс.</span><span class="sxs-lookup"><span data-stu-id="cf162-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="cf162-106">После публикации назначения для учащихся преподаватели не могут удалять ресурсы, помеченные как "Дистрибутетостудентс".</span><span class="sxs-lookup"><span data-stu-id="cf162-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="cf162-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf162-107">Permissions</span></span>
<span data-ttu-id="cf162-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf162-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf162-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf162-110">Permission type</span></span>      | <span data-ttu-id="cf162-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf162-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf162-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf162-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cf162-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf162-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cf162-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf162-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cf162-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf162-115">Not supported.</span></span>  |
|<span data-ttu-id="cf162-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf162-116">Application</span></span> | <span data-ttu-id="cf162-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf162-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cf162-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf162-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cf162-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf162-119">Request headers</span></span>
| <span data-ttu-id="cf162-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf162-120">Header</span></span>       | <span data-ttu-id="cf162-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf162-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf162-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf162-122">Authorization</span></span>  | <span data-ttu-id="cf162-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf162-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf162-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf162-125">Request body</span></span>
<span data-ttu-id="cf162-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf162-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cf162-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf162-127">Response</span></span>
<span data-ttu-id="cf162-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf162-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf162-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cf162-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf162-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf162-131">Request</span></span>
<span data-ttu-id="cf162-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf162-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="cf162-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf162-133">Response</span></span>
<span data-ttu-id="cf162-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf162-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf162-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="cf162-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf162-136">C#</span><span class="sxs-lookup"><span data-stu-id="cf162-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignmentresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf162-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf162-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignmentresource-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cf162-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cf162-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationassignmentresource-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
