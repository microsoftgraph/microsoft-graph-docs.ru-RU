---
title: Добавление преподавателя
description: Добавление преподавателя в класс.
author: mmast-msft
ms.openlocfilehash: 72887960cd43fcbc84ecdf33c3c9cca3e2a0cdd3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361259"
---
# <a name="add-teacher"></a><span data-ttu-id="309b9-103">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="309b9-103">Add teacher</span></span>

> <span data-ttu-id="309b9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="309b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="309b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="309b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="309b9-106">Добавление преподавателя в класс.</span><span class="sxs-lookup"><span data-stu-id="309b9-106">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="309b9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="309b9-107">Permissions</span></span>
<span data-ttu-id="309b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="309b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="309b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="309b9-110">Permission type</span></span>      | <span data-ttu-id="309b9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="309b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="309b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="309b9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="309b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="309b9-113">Not supported.</span></span>  |
|<span data-ttu-id="309b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="309b9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="309b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="309b9-115">Not supported.</span></span>  |
|<span data-ttu-id="309b9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="309b9-116">Application</span></span> | <span data-ttu-id="309b9-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="309b9-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="309b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="309b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="309b9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="309b9-119">Request headers</span></span>
| <span data-ttu-id="309b9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="309b9-120">Header</span></span>       | <span data-ttu-id="309b9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="309b9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="309b9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="309b9-122">Authorization</span></span>  | <span data-ttu-id="309b9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="309b9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="309b9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="309b9-125">Content-Type</span></span>  | <span data-ttu-id="309b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="309b9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="309b9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="309b9-127">Request body</span></span>
<span data-ttu-id="309b9-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="309b9-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="309b9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="309b9-129">Response</span></span>
<span data-ttu-id="309b9-130">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="309b9-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="309b9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="309b9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="309b9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="309b9-132">Request</span></span>
<span data-ttu-id="309b9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="309b9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="309b9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="309b9-134">Response</span></span>
<span data-ttu-id="309b9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="309b9-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="309b9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="309b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
