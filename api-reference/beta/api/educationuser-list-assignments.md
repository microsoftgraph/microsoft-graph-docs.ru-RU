---
title: Перечисление заданий
description: Возвращает список назначений, присвоенных пользователю для всех классов. Это пространство имен утилиты позволяет вызываемой группе находить все назначения учащегося в одном вызове, а не запрашивать назначения у каждого класса. В списке назначений содержится то, что необходимо для получения подробных сведений о назначении из пространства имен класса. Все остальные операции назначения должны использовать пространство имен класса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c660185ec5f0e0c7a2eaed46f5b0cc43499500ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042844"
---
# <a name="list-assignments"></a><span data-ttu-id="10c20-106">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="10c20-106">List assignments</span></span>

<span data-ttu-id="10c20-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10c20-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10c20-108">Возвращает список назначений, присвоенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="10c20-108">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="10c20-109">Это пространство имен утилиты позволяет вызываемой группе находить все назначения учащегося в одном вызове, а не запрашивать назначения у каждого класса.</span><span class="sxs-lookup"><span data-stu-id="10c20-109">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="10c20-110">В списке назначений содержится то, что необходимо для получения подробных сведений о назначении из пространства имен класса.</span><span class="sxs-lookup"><span data-stu-id="10c20-110">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="10c20-111">Все остальные операции назначения должны использовать пространство имен класса.</span><span class="sxs-lookup"><span data-stu-id="10c20-111">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="10c20-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10c20-112">Permissions</span></span>

<span data-ttu-id="10c20-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c20-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10c20-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10c20-115">Permission type</span></span>                        | <span data-ttu-id="10c20-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10c20-116">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="10c20-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10c20-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="10c20-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10c20-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="10c20-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10c20-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10c20-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c20-120">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="10c20-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10c20-121">Application</span></span>                            | <span data-ttu-id="10c20-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c20-122">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="10c20-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10c20-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10c20-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10c20-124">Optional query parameters</span></span>

<span data-ttu-id="10c20-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10c20-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10c20-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10c20-126">Request headers</span></span>

| <span data-ttu-id="10c20-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10c20-127">Header</span></span>        | <span data-ttu-id="10c20-128">Значение</span><span class="sxs-lookup"><span data-stu-id="10c20-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="10c20-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10c20-129">Authorization</span></span> | <span data-ttu-id="10c20-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10c20-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10c20-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10c20-132">Request body</span></span>

<span data-ttu-id="10c20-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10c20-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10c20-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c20-134">Response</span></span>

<span data-ttu-id="10c20-135">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10c20-135">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c20-136">Пример</span><span class="sxs-lookup"><span data-stu-id="10c20-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10c20-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="10c20-137">Request</span></span>
<span data-ttu-id="10c20-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10c20-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```

##### <a name="response"></a><span data-ttu-id="10c20-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c20-139">Response</span></span>

<span data-ttu-id="10c20-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10c20-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="10c20-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10c20-141">**Note:** The response object shown here might be shortened for readability.</span></span>


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