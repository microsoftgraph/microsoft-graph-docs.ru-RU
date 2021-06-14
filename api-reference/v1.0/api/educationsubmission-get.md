---
title: Get educationSubmission
description: 'Извлечение определенной отправки. Объект отправки представляет работу учащегося для назначения. Ресурсы, связанные с отправкой, представляют эту работу. Увидеть и изменить представление может только учащийся, за который назначена отправка. Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем отправкам. '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3188fd2c1bb9643cb9ba8f94621cd08067572b71
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912948"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="0b07d-107">Get educationSubmission</span><span class="sxs-lookup"><span data-stu-id="0b07d-107">Get educationSubmission</span></span>

<span data-ttu-id="0b07d-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b07d-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b07d-109">Извлечение определенной отправки.</span><span class="sxs-lookup"><span data-stu-id="0b07d-109">Retrieve a particular submission.</span></span>

<span data-ttu-id="0b07d-110">Объект отправки представляет работу учащегося для назначения.</span><span class="sxs-lookup"><span data-stu-id="0b07d-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="0b07d-111">Ресурсы, связанные с отправкой, представляют эту работу.</span><span class="sxs-lookup"><span data-stu-id="0b07d-111">Resources associated with the submission represent this work.</span></span> 

<span data-ttu-id="0b07d-112">Только **назначенное Учащемуся** может видеть и изменять отправку.</span><span class="sxs-lookup"><span data-stu-id="0b07d-112">Only the **assignedTo** student can see and modify the submission.</span></span> <span data-ttu-id="0b07d-113">Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем отправкам.</span><span class="sxs-lookup"><span data-stu-id="0b07d-113">A teacher or application with application permissions has full access to all submissions.</span></span>

<span data-ttu-id="0b07d-114">Оценка и отзывы от преподавателя являются частью [образованияOutcome,](../resources/educationoutcome.md) связанного с этим объектом.</span><span class="sxs-lookup"><span data-stu-id="0b07d-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="0b07d-115">Добавить или изменить оценки и отзывы могут только преподаватели или приложения с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="0b07d-115">Only teachers or applications with application permissions can add or change grades and feedback.</span></span> <span data-ttu-id="0b07d-116">Учащиеся не будут видеть оценку или отзывы до тех пор, пока назначение не будет выпущено.</span><span class="sxs-lookup"><span data-stu-id="0b07d-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b07d-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b07d-117">Permissions</span></span>
<span data-ttu-id="0b07d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b07d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b07d-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b07d-120">Permission type</span></span>      | <span data-ttu-id="0b07d-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b07d-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b07d-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b07d-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b07d-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b07d-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="0b07d-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b07d-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0b07d-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b07d-125">Not supported.</span></span>  |
|<span data-ttu-id="0b07d-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b07d-126">Application</span></span> | <span data-ttu-id="0b07d-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b07d-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0b07d-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b07d-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b07d-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b07d-129">Optional query parameters</span></span>
<span data-ttu-id="0b07d-130">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b07d-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b07d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b07d-131">Request headers</span></span>
| <span data-ttu-id="0b07d-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b07d-132">Header</span></span>       | <span data-ttu-id="0b07d-133">Значение</span><span class="sxs-lookup"><span data-stu-id="0b07d-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b07d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b07d-134">Authorization</span></span>  | <span data-ttu-id="0b07d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b07d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b07d-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b07d-137">Request body</span></span>
<span data-ttu-id="0b07d-138">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b07d-138">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0b07d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b07d-139">Response</span></span>
<span data-ttu-id="0b07d-140">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [educationSubmission](../resources/educationsubmission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0b07d-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b07d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0b07d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b07d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b07d-142">Request</span></span>
<span data-ttu-id="0b07d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b07d-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b07d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b07d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/11010/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/33223
```

### <a name="response"></a><span data-ttu-id="0b07d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b07d-145">Response</span></span>
<span data-ttu-id="0b07d-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b07d-146">The following is an example of the response.</span></span> 

><span data-ttu-id="0b07d-147">**Примечания:** Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b07d-147">**Notes:** The response object shown here might be shortened for readability.</span></span> 
>
><span data-ttu-id="0b07d-148">Если [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) еще не был вызван на этот ресурс [educationSubmission,](../resources/educationsubmission.md) свойство **resourcesFolderUrl** `null` является .</span><span class="sxs-lookup"><span data-stu-id="0b07d-148">If [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) has not been called on this [educationSubmission](../resources/educationsubmission.md) resource yet, the **resourcesFolderUrl** property is `null`.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
      "id": "33223",
      "recipient": {
        "userId": "13015"
      },
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Shawn Hughes",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
