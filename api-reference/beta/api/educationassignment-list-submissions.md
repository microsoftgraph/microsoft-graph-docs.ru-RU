---
title: Отправка списка
description: Перечисление всех отправок, связанных с этим назначением. Преподаватель может получить все отправленные данные, пока учащийся сможет получить только те из них, с которыми они сопоставлены.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d0aa4e8119ba1d06d11e703545300411cf70d561
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37724579"
---
# <a name="list-submissions"></a><span data-ttu-id="efd3a-104">Отправка списка</span><span class="sxs-lookup"><span data-stu-id="efd3a-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd3a-105">Перечисление всех отправок, связанных с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="efd3a-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="efd3a-106">Преподаватель может получить все отправленные данные, пока учащийся сможет получить только те из них, с которыми они сопоставлены.</span><span class="sxs-lookup"><span data-stu-id="efd3a-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="efd3a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efd3a-107">Permissions</span></span>
<span data-ttu-id="efd3a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efd3a-110">Permission type</span></span>      | <span data-ttu-id="efd3a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efd3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efd3a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="efd3a-113">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd3a-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="efd3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efd3a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="efd3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd3a-115">Not supported.</span></span>  |
|<span data-ttu-id="efd3a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efd3a-116">Application</span></span> | <span data-ttu-id="efd3a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd3a-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="efd3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efd3a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efd3a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efd3a-119">Optional query parameters</span></span>
<span data-ttu-id="efd3a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="efd3a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efd3a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efd3a-121">Request headers</span></span>
| <span data-ttu-id="efd3a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efd3a-122">Header</span></span>       | <span data-ttu-id="efd3a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="efd3a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="efd3a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efd3a-124">Authorization</span></span>  | <span data-ttu-id="efd3a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efd3a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efd3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efd3a-127">Request body</span></span>
<span data-ttu-id="efd3a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efd3a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="efd3a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="efd3a-129">Response</span></span>
<span data-ttu-id="efd3a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efd3a-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efd3a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="efd3a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efd3a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="efd3a-132">Request</span></span>
<span data-ttu-id="efd3a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efd3a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="efd3a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="efd3a-134">Response</span></span>
<span data-ttu-id="efd3a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="efd3a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="efd3a-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efd3a-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="efd3a-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efd3a-137">All of the properties will be returned from an actual call.</span></span>

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
