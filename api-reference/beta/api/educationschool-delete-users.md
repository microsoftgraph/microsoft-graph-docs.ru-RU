---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47f07b3cba001bee1bd2c978f8a4e660eac43172
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325190"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="3f860-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="3f860-103">Remove educationUser from an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f860-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="3f860-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f860-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f860-105">Permissions</span></span>
<span data-ttu-id="3f860-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f860-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f860-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f860-108">Permission type</span></span>      | <span data-ttu-id="3f860-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f860-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f860-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f860-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3f860-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f860-111">Not supported.</span></span>  |
|<span data-ttu-id="3f860-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f860-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3f860-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f860-113">Not supported.</span></span>  |
|<span data-ttu-id="3f860-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f860-114">Application</span></span> | <span data-ttu-id="3f860-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f860-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3f860-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f860-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/<id>/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3f860-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f860-117">Request headers</span></span>
| <span data-ttu-id="3f860-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f860-118">Header</span></span>       | <span data-ttu-id="3f860-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3f860-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f860-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f860-120">Authorization</span></span>  | <span data-ttu-id="3f860-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f860-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f860-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f860-123">Request body</span></span>
<span data-ttu-id="3f860-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f860-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3f860-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f860-125">Response</span></span>
<span data-ttu-id="3f860-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="3f860-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f860-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3f860-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f860-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f860-128">Request</span></span>
<span data-ttu-id="3f860-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f860-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="3f860-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f860-130">Response</span></span>
<span data-ttu-id="3f860-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f860-131">The following is an example of the response.</span></span> 
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
