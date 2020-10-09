---
title: Отправка списка
description: Перечисление всех отправок, связанных с этим назначением. Преподаватель может получить все отправленные данные, пока учащийся сможет получить только те из них, с которыми они сопоставлены.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1563a4fade4aab474714609ee479a5a11f5c3867
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403617"
---
# <a name="list-submissions"></a><span data-ttu-id="2e4bf-104">Отправка списка</span><span class="sxs-lookup"><span data-stu-id="2e4bf-104">List submissions</span></span>

<span data-ttu-id="2e4bf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4bf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e4bf-106">Перечисление всех отправок, связанных с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="2e4bf-107">Преподаватель может получить все отправленные данные, пока учащийся сможет получить только те из них, с которыми они сопоставлены.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-107">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e4bf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e4bf-108">Permissions</span></span>
<span data-ttu-id="2e4bf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e4bf-111">Permission type</span></span>      | <span data-ttu-id="2e4bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e4bf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e4bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e4bf-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e4bf-114">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4bf-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2e4bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e4bf-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2e4bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-116">Not supported.</span></span>  |
|<span data-ttu-id="2e4bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e4bf-117">Application</span></span> | <span data-ttu-id="2e4bf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-118">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e4bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e4bf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e4bf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e4bf-120">Optional query parameters</span></span>
<span data-ttu-id="2e4bf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e4bf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e4bf-122">Request headers</span></span>
| <span data-ttu-id="2e4bf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e4bf-123">Header</span></span>       | <span data-ttu-id="2e4bf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2e4bf-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e4bf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e4bf-125">Authorization</span></span>  | <span data-ttu-id="2e4bf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e4bf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e4bf-128">Request body</span></span>
<span data-ttu-id="2e4bf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e4bf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4bf-130">Response</span></span>
<span data-ttu-id="2e4bf-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e4bf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2e4bf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e4bf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e4bf-133">Request</span></span>
<span data-ttu-id="2e4bf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="2e4bf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4bf-135">Response</span></span>
<span data-ttu-id="2e4bf-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-136">The following is an example of the response.</span></span> 

><span data-ttu-id="2e4bf-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2e4bf-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e4bf-138">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->