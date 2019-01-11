---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4249ae683cab4dc2c9d42699f67dfbd5ca9c3ece
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865550"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="0c289-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="0c289-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="0c289-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="0c289-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c289-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c289-105">Permissions</span></span>
<span data-ttu-id="0c289-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c289-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c289-108">Permission type</span></span>      | <span data-ttu-id="0c289-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c289-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c289-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c289-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c289-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c289-111">Not supported.</span></span>  |
|<span data-ttu-id="0c289-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c289-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c289-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c289-113">Not supported.</span></span>  |
|<span data-ttu-id="0c289-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c289-114">Application</span></span> | <span data-ttu-id="0c289-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c289-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c289-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c289-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0c289-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c289-117">Request headers</span></span>
| <span data-ttu-id="0c289-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c289-118">Header</span></span>       | <span data-ttu-id="0c289-119">Значение</span><span class="sxs-lookup"><span data-stu-id="0c289-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c289-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c289-120">Authorization</span></span>  | <span data-ttu-id="0c289-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c289-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c289-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c289-123">Request body</span></span>
<span data-ttu-id="0c289-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c289-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0c289-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c289-125">Response</span></span>
<span data-ttu-id="0c289-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="0c289-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c289-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0c289-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c289-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c289-128">Request</span></span>
<span data-ttu-id="0c289-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c289-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="0c289-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c289-130">Response</span></span>
<span data-ttu-id="0c289-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0c289-131">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
