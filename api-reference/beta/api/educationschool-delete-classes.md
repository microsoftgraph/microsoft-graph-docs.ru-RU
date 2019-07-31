---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15ab30facb9c8d762e05c37ea8230b3178ab86f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955224"
---
# <a name="remove-educationclass"></a><span data-ttu-id="0d6b6-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="0d6b6-103">Remove educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d6b6-104">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d6b6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d6b6-105">Permissions</span></span>
<span data-ttu-id="0d6b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d6b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d6b6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d6b6-108">Permission type</span></span>      | <span data-ttu-id="0d6b6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d6b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d6b6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d6b6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0d6b6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-111">Not supported.</span></span>  |
|<span data-ttu-id="0d6b6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d6b6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0d6b6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-113">Not supported.</span></span>  |
|<span data-ttu-id="0d6b6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d6b6-114">Application</span></span> | <span data-ttu-id="0d6b6-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d6b6-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0d6b6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d6b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0d6b6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d6b6-117">Request headers</span></span>
| <span data-ttu-id="0d6b6-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d6b6-118">Header</span></span>       | <span data-ttu-id="0d6b6-119">Значение</span><span class="sxs-lookup"><span data-stu-id="0d6b6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d6b6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d6b6-120">Authorization</span></span>  | <span data-ttu-id="0d6b6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d6b6-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d6b6-123">Request body</span></span>
<span data-ttu-id="0d6b6-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0d6b6-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d6b6-125">Response</span></span>
<span data-ttu-id="0d6b6-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d6b6-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0d6b6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d6b6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d6b6-128">Request</span></span>
<span data-ttu-id="0d6b6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="0d6b6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d6b6-130">Response</span></span>
<span data-ttu-id="0d6b6-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d6b6-131">The following is an example of the response.</span></span> 

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
  "suppressions": []
}
-->
