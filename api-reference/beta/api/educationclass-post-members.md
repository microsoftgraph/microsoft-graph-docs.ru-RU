---
title: Добавление учащегося
description: Добавление участника курса.
ms.openlocfilehash: 0b748a924de1f882372c0117f94d0de06f64dbc9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075685"
---
# <a name="add-a-student"></a><span data-ttu-id="93654-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="93654-103">Add a student</span></span>

> <span data-ttu-id="93654-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93654-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93654-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93654-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93654-106">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="93654-106">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="93654-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93654-107">Permissions</span></span>
<span data-ttu-id="93654-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93654-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93654-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93654-110">Permission type</span></span>      | <span data-ttu-id="93654-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93654-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93654-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93654-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="93654-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93654-113">Not supported.</span></span>  |
|<span data-ttu-id="93654-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93654-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93654-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93654-115">Not supported.</span></span>  |
|<span data-ttu-id="93654-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="93654-116">Application</span></span> | <span data-ttu-id="93654-117">EduRoster.ReadWrite.All, а также Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="93654-117">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="93654-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93654-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="93654-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93654-119">Request headers</span></span>
| <span data-ttu-id="93654-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93654-120">Header</span></span>       | <span data-ttu-id="93654-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93654-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93654-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93654-122">Authorization</span></span>  | <span data-ttu-id="93654-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93654-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="93654-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93654-125">Content-Type</span></span>  | <span data-ttu-id="93654-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93654-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93654-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93654-127">Request body</span></span>
<span data-ttu-id="93654-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93654-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="93654-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="93654-129">Response</span></span>
<span data-ttu-id="93654-130">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93654-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93654-131">Пример</span><span class="sxs-lookup"><span data-stu-id="93654-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93654-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="93654-132">Request</span></span>
<span data-ttu-id="93654-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93654-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="93654-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="93654-134">Response</span></span>
<span data-ttu-id="93654-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93654-135">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
