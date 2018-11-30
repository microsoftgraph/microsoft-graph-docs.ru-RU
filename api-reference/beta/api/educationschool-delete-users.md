---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
ms.openlocfilehash: 05ca8d1940580ac2897c842905a754c37a8c8814
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077899"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="ba05f-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="ba05f-103">Remove educationUser from an educationSchool</span></span>

> <span data-ttu-id="ba05f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba05f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba05f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba05f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba05f-106">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ba05f-106">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba05f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba05f-107">Permissions</span></span>
<span data-ttu-id="ba05f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba05f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba05f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba05f-110">Permission type</span></span>      | <span data-ttu-id="ba05f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba05f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba05f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba05f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ba05f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba05f-113">Not supported.</span></span>  |
|<span data-ttu-id="ba05f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba05f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ba05f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba05f-115">Not supported.</span></span>  |
|<span data-ttu-id="ba05f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba05f-116">Application</span></span> | <span data-ttu-id="ba05f-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba05f-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba05f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba05f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/<id>/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ba05f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba05f-119">Request headers</span></span>
| <span data-ttu-id="ba05f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba05f-120">Header</span></span>       | <span data-ttu-id="ba05f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba05f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba05f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba05f-122">Authorization</span></span>  | <span data-ttu-id="ba05f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba05f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba05f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba05f-125">Request body</span></span>
<span data-ttu-id="ba05f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba05f-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ba05f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba05f-127">Response</span></span>
<span data-ttu-id="ba05f-128">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="ba05f-128">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba05f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ba05f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba05f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba05f-130">Request</span></span>
<span data-ttu-id="ba05f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba05f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="ba05f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba05f-132">Response</span></span>
<span data-ttu-id="ba05f-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ba05f-133">The following is an example of the response.</span></span> 
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