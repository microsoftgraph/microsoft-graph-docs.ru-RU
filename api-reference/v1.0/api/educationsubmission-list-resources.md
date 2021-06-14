---
title: Список ресурсов отправки
description: Список ресурсов, связанных с отправкой.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d291ac67988d3960c70df1f8183b0c8989ce008
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911564"
---
# <a name="list-submission-resources"></a><span data-ttu-id="b0100-103">Список ресурсов отправки</span><span class="sxs-lookup"><span data-stu-id="b0100-103">List submission resources</span></span>

<span data-ttu-id="b0100-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0100-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0100-105">Список ресурсов, связанных с [отправкой.](../resources/educationsubmission.md)</span><span class="sxs-lookup"><span data-stu-id="b0100-105">List the resources associated with a [submission](../resources/educationsubmission.md).</span></span> 

<span data-ttu-id="b0100-106">Объект **submissionResource** — это оболочка вокруг фактического объекта ресурса, над который работает студент.</span><span class="sxs-lookup"><span data-stu-id="b0100-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="b0100-107">Оболочка также включает указатель на ресурсы назначения, если он был скопирован из назначения во время процесса назначения.</span><span class="sxs-lookup"><span data-stu-id="b0100-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="b0100-108">Эти ресурсы являются рабочей копией назначения.</span><span class="sxs-lookup"><span data-stu-id="b0100-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="b0100-109">**SubmittedResources —** это ресурсы, официально отправленные для оценки.</span><span class="sxs-lookup"><span data-stu-id="b0100-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0100-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0100-110">Permissions</span></span>

<span data-ttu-id="b0100-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0100-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0100-113">Permission type</span></span>                        | <span data-ttu-id="b0100-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0100-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b0100-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0100-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0100-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0100-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b0100-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0100-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0100-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0100-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="b0100-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="b0100-119">Application</span></span>                            | <span data-ttu-id="b0100-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0100-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0100-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0100-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0100-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0100-122">Optional query parameters</span></span>

<span data-ttu-id="b0100-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b0100-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0100-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0100-124">Request headers</span></span>

| <span data-ttu-id="b0100-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0100-125">Header</span></span>        | <span data-ttu-id="b0100-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b0100-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b0100-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0100-127">Authorization</span></span> | <span data-ttu-id="b0100-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0100-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0100-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0100-130">Request body</span></span>

<span data-ttu-id="b0100-131">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0100-131">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0100-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0100-132">Response</span></span>

<span data-ttu-id="b0100-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0100-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0100-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b0100-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0100-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0100-135">Request</span></span>

<span data-ttu-id="b0100-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0100-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

### <a name="response"></a><span data-ttu-id="b0100-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0100-137">Response</span></span>

<span data-ttu-id="b0100-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b0100-138">The following is an example of the response.</span></span> 

><span data-ttu-id="b0100-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0100-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
