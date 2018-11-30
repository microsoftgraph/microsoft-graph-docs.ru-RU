---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
ms.openlocfilehash: cdccc9147f8a6eb0ba8bd2c79b8ce28ecddb514f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075698"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="9e408-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="9e408-103">Add educationUser to an educationSchool</span></span>

> <span data-ttu-id="9e408-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e408-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e408-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e408-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e408-106">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="9e408-106">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e408-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e408-107">Permissions</span></span>
<span data-ttu-id="9e408-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e408-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e408-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e408-110">Permission type</span></span>      | <span data-ttu-id="9e408-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e408-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e408-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e408-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9e408-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e408-113">Not supported.</span></span>  |
|<span data-ttu-id="9e408-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e408-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9e408-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e408-115">Not supported.</span></span>  |
|<span data-ttu-id="9e408-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e408-116">Application</span></span> | <span data-ttu-id="9e408-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e408-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9e408-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e408-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9e408-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e408-119">Request headers</span></span>
| <span data-ttu-id="9e408-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e408-120">Header</span></span>       | <span data-ttu-id="9e408-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9e408-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e408-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e408-122">Authorization</span></span>  | <span data-ttu-id="9e408-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e408-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9e408-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e408-125">Content-Type</span></span>  | <span data-ttu-id="9e408-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e408-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e408-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e408-127">Request body</span></span>
<span data-ttu-id="9e408-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e408-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9e408-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e408-129">Response</span></span>
<span data-ttu-id="9e408-130">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e408-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e408-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e408-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e408-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e408-132">Request</span></span>
<span data-ttu-id="9e408-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e408-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/<id>/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="9e408-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e408-134">Response</span></span>
<span data-ttu-id="9e408-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9e408-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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