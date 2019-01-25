---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34c7531f3c45caf2a26099fc150666ff6a7899ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517192"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="02209-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="02209-103">Remove educationUser from an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02209-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="02209-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="02209-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02209-105">Permissions</span></span>
<span data-ttu-id="02209-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02209-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02209-108">Permission type</span></span>      | <span data-ttu-id="02209-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02209-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02209-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02209-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="02209-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02209-111">Not supported.</span></span>  |
|<span data-ttu-id="02209-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02209-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02209-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02209-113">Not supported.</span></span>  |
|<span data-ttu-id="02209-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02209-114">Application</span></span> | <span data-ttu-id="02209-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02209-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="02209-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02209-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/<id>/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="02209-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02209-117">Request headers</span></span>
| <span data-ttu-id="02209-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02209-118">Header</span></span>       | <span data-ttu-id="02209-119">Значение</span><span class="sxs-lookup"><span data-stu-id="02209-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02209-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02209-120">Authorization</span></span>  | <span data-ttu-id="02209-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02209-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02209-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02209-123">Request body</span></span>
<span data-ttu-id="02209-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02209-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="02209-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="02209-125">Response</span></span>
<span data-ttu-id="02209-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="02209-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="02209-127">Пример</span><span class="sxs-lookup"><span data-stu-id="02209-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02209-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="02209-128">Request</span></span>
<span data-ttu-id="02209-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02209-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="02209-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="02209-130">Response</span></span>
<span data-ttu-id="02209-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02209-131">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-delete-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
