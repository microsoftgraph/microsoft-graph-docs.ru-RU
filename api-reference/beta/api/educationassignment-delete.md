---
title: Удаление educationAssignment
description: Удаление существующего назначения. Удалять назначения могут только преподаватели внутри класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2356330a75558ea88b94c9266fb2d4a387e87b59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464742"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="cbf72-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="cbf72-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbf72-105">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="cbf72-105">Delete an existing assignment.</span></span> <span data-ttu-id="cbf72-106">Удалять назначения могут только преподаватели внутри класса.</span><span class="sxs-lookup"><span data-stu-id="cbf72-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbf72-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbf72-107">Permissions</span></span>
<span data-ttu-id="cbf72-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbf72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbf72-110">Permission type</span></span>      | <span data-ttu-id="cbf72-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbf72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbf72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbf72-112">Delegated (work or school account)</span></span>| <span data-ttu-id="cbf72-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbf72-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="cbf72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbf72-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="cbf72-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbf72-115">Not Supported.</span></span> |
|<span data-ttu-id="cbf72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbf72-116">Application</span></span> | <span data-ttu-id="cbf72-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbf72-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cbf72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbf72-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="cbf72-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbf72-119">Request headers</span></span>
| <span data-ttu-id="cbf72-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbf72-120">Header</span></span>       | <span data-ttu-id="cbf72-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cbf72-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbf72-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbf72-122">Authorization</span></span>  | <span data-ttu-id="cbf72-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbf72-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbf72-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbf72-125">Request body</span></span>
<span data-ttu-id="cbf72-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbf72-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cbf72-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf72-127">Response</span></span>
<span data-ttu-id="cbf72-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cbf72-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf72-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cbf72-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbf72-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbf72-131">Request</span></span>
<span data-ttu-id="cbf72-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbf72-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="cbf72-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf72-133">Response</span></span>
<span data-ttu-id="cbf72-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbf72-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
