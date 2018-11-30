---
title: Удаление учащегося
description: Удаляет educationUser из educationClass.
ms.openlocfilehash: 6729622a07f36bd08e9f5e8a32312aa38582b490
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076621"
---
# <a name="remove-a-student"></a><span data-ttu-id="9ce1b-103">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="9ce1b-103">Remove a student</span></span>

> <span data-ttu-id="9ce1b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ce1b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ce1b-106">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="9ce1b-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="9ce1b-107">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="9ce1b-108">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="9ce1b-109">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass-list-teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce1b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce1b-110">Permissions</span></span>
<span data-ttu-id="9ce1b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce1b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce1b-113">Permission type</span></span>      | <span data-ttu-id="9ce1b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce1b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ce1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-116">Not supported.</span></span>  |
|<span data-ttu-id="9ce1b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ce1b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-118">Not supported.</span></span>  |
|<span data-ttu-id="9ce1b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ce1b-119">Application</span></span> | <span data-ttu-id="9ce1b-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce1b-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ce1b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ce1b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9ce1b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ce1b-122">Request headers</span></span>
| <span data-ttu-id="9ce1b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ce1b-123">Header</span></span>       | <span data-ttu-id="9ce1b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9ce1b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ce1b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ce1b-125">Authorization</span></span>  | <span data-ttu-id="9ce1b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ce1b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ce1b-128">Request body</span></span>
<span data-ttu-id="9ce1b-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9ce1b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce1b-130">Response</span></span>
<span data-ttu-id="9ce1b-131">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce1b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9ce1b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ce1b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce1b-133">Request</span></span>
<span data-ttu-id="9ce1b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="9ce1b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ce1b-135">Response</span></span>
<span data-ttu-id="9ce1b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-136">The following is an example of the response.</span></span> 
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
