---
title: 'educationAssignment: публикация'
description: Это действие изменяет состояние назначения его исходное состояние черновика для опубликованного состояние. Только преподаватель в классе можно позвонить. После назначения находится в состоянии черновиков, студентов не отображается как назначения, а также будет ли любые объекты отправки. При вызове этот интерфейс API для создания объектов отправки и назначения в списке учащегося.
localization_priority: Normal
ms.openlocfilehash: 09261da506113f53c6b6b9ff98af69c7dba4c784
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854742"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="8d27f-106">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="8d27f-106">educationAssignment: publish</span></span>

> <span data-ttu-id="8d27f-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d27f-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d27f-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d27f-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d27f-109">Это действие изменяет состояние назначения его исходное состояние черновика для опубликованного состояние.</span><span class="sxs-lookup"><span data-stu-id="8d27f-109">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="8d27f-110">Только преподаватель в классе можно позвонить.</span><span class="sxs-lookup"><span data-stu-id="8d27f-110">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="8d27f-111">После назначения находится в состоянии черновиков, студентов не отображается как назначения, а также будет ли любые объекты отправки.</span><span class="sxs-lookup"><span data-stu-id="8d27f-111">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="8d27f-112">При вызове этот интерфейс API для создания объектов отправки и назначения в списке учащегося.</span><span class="sxs-lookup"><span data-stu-id="8d27f-112">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d27f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d27f-113">Permissions</span></span>
<span data-ttu-id="8d27f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d27f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d27f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d27f-116">Permission type</span></span>      | <span data-ttu-id="8d27f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d27f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d27f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d27f-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d27f-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d27f-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8d27f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d27f-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8d27f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d27f-121">Not supported.</span></span>  |
|<span data-ttu-id="8d27f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d27f-122">Application</span></span> | <span data-ttu-id="8d27f-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d27f-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d27f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d27f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="8d27f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d27f-125">Request headers</span></span>
| <span data-ttu-id="8d27f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d27f-126">Header</span></span>       | <span data-ttu-id="8d27f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="8d27f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d27f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d27f-128">Authorization</span></span>  | <span data-ttu-id="8d27f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d27f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d27f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d27f-131">Request body</span></span>
<span data-ttu-id="8d27f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d27f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d27f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d27f-133">Response</span></span>
<span data-ttu-id="8d27f-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d27f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d27f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8d27f-136">Example</span></span>
<span data-ttu-id="8d27f-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8d27f-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d27f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d27f-138">Request</span></span>
<span data-ttu-id="8d27f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d27f-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="8d27f-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d27f-140">Response</span></span>
<span data-ttu-id="8d27f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d27f-141">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
