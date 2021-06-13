---
title: Список назначений пользователя
description: Возвращает список назначений, присвоенных пользователю для всех классов.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d92a6f32a3b986f9fb0e3b24b6537897f23ca2c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911769"
---
# <a name="list-assignments-of-a-user"></a><span data-ttu-id="d6ea4-103">Список назначений пользователя</span><span class="sxs-lookup"><span data-stu-id="d6ea4-103">List assignments of a user</span></span>

<span data-ttu-id="d6ea4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ea4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6ea4-105">Возвращает список назначений, присвоенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-105">Returns a list of assignments assigned to a user for all classes.</span></span> 

<span data-ttu-id="d6ea4-106">Это пространство имен утилиты позволяет вызываемой группе находить все назначения учащегося в одном вызове, а не запрашивать назначения у каждого класса.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-106">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="d6ea4-107">В списке назначений содержится то, что необходимо для получения подробных сведений о назначении из пространства имен класса.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-107">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="d6ea4-108">Все остальные операции назначения должны использовать пространство имен класса.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-108">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6ea4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6ea4-109">Permissions</span></span>

<span data-ttu-id="d6ea4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6ea4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6ea4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6ea4-112">Permission type</span></span>                        | <span data-ttu-id="d6ea4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6ea4-113">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d6ea4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6ea4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6ea4-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6ea4-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d6ea4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6ea4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ea4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-117">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="d6ea4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6ea4-118">Application</span></span>                            | <span data-ttu-id="d6ea4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-119">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="d6ea4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6ea4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6ea4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6ea4-121">Optional query parameters</span></span>

<span data-ttu-id="d6ea4-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6ea4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6ea4-123">Request headers</span></span>

| <span data-ttu-id="d6ea4-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6ea4-124">Header</span></span>        | <span data-ttu-id="d6ea4-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d6ea4-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d6ea4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6ea4-126">Authorization</span></span> | <span data-ttu-id="d6ea4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6ea4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6ea4-129">Request body</span></span>

<span data-ttu-id="d6ea4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6ea4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6ea4-131">Response</span></span>

<span data-ttu-id="d6ea4-132">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6ea4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d6ea4-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6ea4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6ea4-134">Request</span></span>
<span data-ttu-id="d6ea4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_me_assignments"
}-->

```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```

##### <a name="response"></a><span data-ttu-id="d6ea4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6ea4-136">Response</span></span>

<span data-ttu-id="d6ea4-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-137">The following is an example of the response.</span></span> 

> <span data-ttu-id="d6ea4-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d6ea4-138">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "closeDateTime": "2014-01-11T00:00:00Z",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->