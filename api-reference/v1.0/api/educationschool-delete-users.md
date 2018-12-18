---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
ms.openlocfilehash: c8fc91aafa1de22d156d077b51bb081f8f940f00
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336773"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="170d7-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="170d7-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="170d7-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="170d7-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="170d7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="170d7-105">Permissions</span></span>
<span data-ttu-id="170d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="170d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="170d7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="170d7-108">Permission type</span></span>      | <span data-ttu-id="170d7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="170d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170d7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="170d7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="170d7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="170d7-111">Not supported.</span></span>  |
|<span data-ttu-id="170d7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="170d7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="170d7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="170d7-113">Not supported.</span></span>  |
|<span data-ttu-id="170d7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="170d7-114">Application</span></span> | <span data-ttu-id="170d7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d7-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="170d7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="170d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="170d7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="170d7-117">Request headers</span></span>
| <span data-ttu-id="170d7-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="170d7-118">Header</span></span>       | <span data-ttu-id="170d7-119">Значение</span><span class="sxs-lookup"><span data-stu-id="170d7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="170d7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="170d7-120">Authorization</span></span>  | <span data-ttu-id="170d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="170d7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="170d7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="170d7-123">Request body</span></span>
<span data-ttu-id="170d7-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="170d7-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="170d7-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="170d7-125">Response</span></span>
<span data-ttu-id="170d7-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="170d7-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="170d7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="170d7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="170d7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="170d7-128">Request</span></span>
<span data-ttu-id="170d7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="170d7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="170d7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="170d7-130">Response</span></span>
<span data-ttu-id="170d7-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="170d7-131">The following is an example of the response.</span></span> 
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