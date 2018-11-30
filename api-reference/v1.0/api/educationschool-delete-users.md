---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
ms.openlocfilehash: dbc58a0cde4406fb28323bedf02a1902998e9b0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026837"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="ee538-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="ee538-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="ee538-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ee538-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee538-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee538-105">Permissions</span></span>
<span data-ttu-id="ee538-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee538-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee538-108">Permission type</span></span>      | <span data-ttu-id="ee538-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee538-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee538-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee538-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ee538-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee538-111">Not supported.</span></span>  |
|<span data-ttu-id="ee538-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee538-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ee538-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee538-113">Not supported.</span></span>  |
|<span data-ttu-id="ee538-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee538-114">Application</span></span> | <span data-ttu-id="ee538-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee538-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ee538-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee538-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ee538-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee538-117">Request headers</span></span>
| <span data-ttu-id="ee538-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee538-118">Header</span></span>       | <span data-ttu-id="ee538-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ee538-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ee538-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee538-120">Authorization</span></span>  | <span data-ttu-id="ee538-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee538-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee538-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee538-123">Request body</span></span>
<span data-ttu-id="ee538-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee538-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ee538-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee538-125">Response</span></span>
<span data-ttu-id="ee538-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="ee538-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee538-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ee538-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee538-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee538-128">Request</span></span>
<span data-ttu-id="ee538-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee538-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="ee538-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee538-130">Response</span></span>
<span data-ttu-id="ee538-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee538-131">The following is an example of the response.</span></span> 
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