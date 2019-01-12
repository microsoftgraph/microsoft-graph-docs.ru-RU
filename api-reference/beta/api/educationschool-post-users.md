---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 13c7eda5546f460da73d4359b064868ac41eb267
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979994"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="d134d-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="d134d-103">Add educationUser to an educationSchool</span></span>

> <span data-ttu-id="d134d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d134d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d134d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d134d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d134d-106">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="d134d-106">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d134d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d134d-107">Permissions</span></span>
<span data-ttu-id="d134d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d134d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d134d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d134d-110">Permission type</span></span>      | <span data-ttu-id="d134d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d134d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d134d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d134d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d134d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d134d-113">Not supported.</span></span>  |
|<span data-ttu-id="d134d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d134d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d134d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d134d-115">Not supported.</span></span>  |
|<span data-ttu-id="d134d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d134d-116">Application</span></span> | <span data-ttu-id="d134d-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d134d-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d134d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d134d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d134d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d134d-119">Request headers</span></span>
| <span data-ttu-id="d134d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d134d-120">Header</span></span>       | <span data-ttu-id="d134d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d134d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d134d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d134d-122">Authorization</span></span>  | <span data-ttu-id="d134d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d134d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d134d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d134d-125">Content-Type</span></span>  | <span data-ttu-id="d134d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d134d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d134d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d134d-127">Request body</span></span>
<span data-ttu-id="d134d-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d134d-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d134d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d134d-129">Response</span></span>
<span data-ttu-id="d134d-130">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d134d-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d134d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d134d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d134d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d134d-132">Request</span></span>
<span data-ttu-id="d134d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d134d-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d134d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d134d-134">Response</span></span>
<span data-ttu-id="d134d-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d134d-135">The following is an example of the response.</span></span> 

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
