---
title: Удаление Едукатионкатегори
description: Удаление существующей категории.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c68f4a9950437ddcebc0cd40237bef07c597648
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457917"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="5992d-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="5992d-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5992d-104">Удаление существующей категории.</span><span class="sxs-lookup"><span data-stu-id="5992d-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="5992d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5992d-105">Permissions</span></span>
<span data-ttu-id="5992d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5992d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5992d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5992d-108">Permission type</span></span>      | <span data-ttu-id="5992d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5992d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5992d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5992d-110">Delegated (work or school account)</span></span>| <span data-ttu-id="5992d-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5992d-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5992d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5992d-112">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="5992d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5992d-113">Not Supported.</span></span> |
|<span data-ttu-id="5992d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5992d-114">Application</span></span> | <span data-ttu-id="5992d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5992d-115">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5992d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5992d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignmentCategories/<id>
```
## <a name="request-headers"></a><span data-ttu-id="5992d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5992d-117">Request headers</span></span>
| <span data-ttu-id="5992d-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5992d-118">Header</span></span>       | <span data-ttu-id="5992d-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5992d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5992d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5992d-120">Authorization</span></span>  | <span data-ttu-id="5992d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5992d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5992d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5992d-123">Request body</span></span>
<span data-ttu-id="5992d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5992d-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5992d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5992d-125">Response</span></span>
<span data-ttu-id="5992d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5992d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5992d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5992d-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="5992d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5992d-129">Request</span></span>
<span data-ttu-id="5992d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5992d-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
### <a name="response"></a><span data-ttu-id="5992d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5992d-131">Response</span></span>
<span data-ttu-id="5992d-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5992d-132">The following is an example of the response.</span></span> 


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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
