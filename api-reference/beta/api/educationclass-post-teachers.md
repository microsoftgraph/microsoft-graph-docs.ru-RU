---
title: Добавление преподавателя
description: Добавление преподавателя в класс.
ms.openlocfilehash: a842aeff30b4911b469e9ae44cb6cedbee02db38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075022"
---
# <a name="add-teacher"></a><span data-ttu-id="a8aca-103">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="a8aca-103">Add teacher</span></span>

> <span data-ttu-id="a8aca-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8aca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8aca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8aca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8aca-106">Добавление преподавателя в класс.</span><span class="sxs-lookup"><span data-stu-id="a8aca-106">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8aca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8aca-107">Permissions</span></span>
<span data-ttu-id="a8aca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8aca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8aca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8aca-110">Permission type</span></span>      | <span data-ttu-id="a8aca-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8aca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8aca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8aca-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a8aca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8aca-113">Not supported.</span></span>  |
|<span data-ttu-id="a8aca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8aca-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a8aca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8aca-115">Not supported.</span></span>  |
|<span data-ttu-id="a8aca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8aca-116">Application</span></span> | <span data-ttu-id="a8aca-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8aca-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a8aca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8aca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a8aca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8aca-119">Request headers</span></span>
| <span data-ttu-id="a8aca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8aca-120">Header</span></span>       | <span data-ttu-id="a8aca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a8aca-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8aca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8aca-122">Authorization</span></span>  | <span data-ttu-id="a8aca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8aca-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a8aca-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8aca-125">Content-Type</span></span>  | <span data-ttu-id="a8aca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8aca-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8aca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8aca-127">Request body</span></span>
<span data-ttu-id="a8aca-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8aca-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a8aca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8aca-129">Response</span></span>
<span data-ttu-id="a8aca-130">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8aca-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8aca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a8aca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8aca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8aca-132">Request</span></span>
<span data-ttu-id="a8aca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8aca-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a8aca-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8aca-134">Response</span></span>
<span data-ttu-id="a8aca-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8aca-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="a8aca-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8aca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
