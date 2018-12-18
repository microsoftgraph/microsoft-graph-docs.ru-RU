---
title: Удаление educationAssignmentResource
description: .
author: dipakboyed
ms.openlocfilehash: 304ec56c8b2da36626f226104568cd353e58e88b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322647"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="da8fd-103">Удаление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="da8fd-103">Delete educationAssignmentResource</span></span>

> <span data-ttu-id="da8fd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da8fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da8fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da8fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da8fd-106">Удалите ресурс из назначения.</span><span class="sxs-lookup"><span data-stu-id="da8fd-106">Delete a resource from an assignment.</span></span> <span data-ttu-id="da8fd-107">Учителя только в классе можно удалить ресурс.</span><span class="sxs-lookup"><span data-stu-id="da8fd-107">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="da8fd-108">После публикации назначения студентов учителя нельзя удалить ресурсы, которые помечены как «distributeToStudents».</span><span class="sxs-lookup"><span data-stu-id="da8fd-108">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="da8fd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da8fd-109">Permissions</span></span>
<span data-ttu-id="da8fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da8fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da8fd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da8fd-112">Permission type</span></span>      | <span data-ttu-id="da8fd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da8fd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da8fd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da8fd-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="da8fd-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da8fd-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="da8fd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da8fd-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da8fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da8fd-117">Not supported.</span></span>  |
|<span data-ttu-id="da8fd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da8fd-118">Application</span></span> | <span data-ttu-id="da8fd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da8fd-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da8fd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da8fd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="da8fd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da8fd-121">Request headers</span></span>
| <span data-ttu-id="da8fd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da8fd-122">Header</span></span>       | <span data-ttu-id="da8fd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="da8fd-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da8fd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da8fd-124">Authorization</span></span>  | <span data-ttu-id="da8fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da8fd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da8fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da8fd-127">Request body</span></span>
<span data-ttu-id="da8fd-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da8fd-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="da8fd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="da8fd-129">Response</span></span>
<span data-ttu-id="da8fd-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da8fd-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da8fd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="da8fd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da8fd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="da8fd-133">Request</span></span>
<span data-ttu-id="da8fd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da8fd-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="da8fd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="da8fd-135">Response</span></span>
<span data-ttu-id="da8fd-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da8fd-136">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->