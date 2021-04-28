---
title: Get educationSubmission
description: 'Извлечение определенной отправки. Объект отправки представляет работу учащегося для назначения. Ресурсы, связанные с отправкой, представляют эту работу. Увидеть и изменить представление может только учащийся, за который назначена отправка. Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем отправкам. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 164428bb5e1a250a3f5e2edafdd859f4ea4361a8
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061828"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="57158-107">Get educationSubmission</span><span class="sxs-lookup"><span data-stu-id="57158-107">Get educationSubmission</span></span>

<span data-ttu-id="57158-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57158-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57158-109">Извлечение определенной отправки.</span><span class="sxs-lookup"><span data-stu-id="57158-109">Retrieve a particular submission.</span></span> <span data-ttu-id="57158-110">Объект отправки представляет работу учащегося для назначения.</span><span class="sxs-lookup"><span data-stu-id="57158-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="57158-111">Ресурсы, связанные с отправкой, представляют эту работу.</span><span class="sxs-lookup"><span data-stu-id="57158-111">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="57158-112">Увидеть и изменить представление может только учащийся, за который назначена отправка.</span><span class="sxs-lookup"><span data-stu-id="57158-112">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="57158-113">Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем отправкам.</span><span class="sxs-lookup"><span data-stu-id="57158-113">A teacher or application with application permissions has full access to all submissions.</span></span>

<span data-ttu-id="57158-114">Оценка и отзывы от преподавателя являются частью [образованияOutcome,](../resources/educationoutcome.md) связанного с этим объектом.</span><span class="sxs-lookup"><span data-stu-id="57158-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="57158-115">Добавить или изменить оценки и отзывы могут только преподаватели или приложения с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="57158-115">Only teachers or applications with application permissions can add or change grades and feedback.</span></span> <span data-ttu-id="57158-116">Учащиеся не будут видеть оценку или отзывы до тех пор, пока назначение не будет выпущено.</span><span class="sxs-lookup"><span data-stu-id="57158-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="57158-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57158-117">Permissions</span></span>
<span data-ttu-id="57158-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57158-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57158-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57158-120">Permission type</span></span>      | <span data-ttu-id="57158-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57158-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57158-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57158-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="57158-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57158-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="57158-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57158-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="57158-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57158-125">Not supported.</span></span>  |
|<span data-ttu-id="57158-126">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="57158-126">Application\*</span></span> | <span data-ttu-id="57158-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57158-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="57158-128">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="57158-128">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="57158-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57158-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57158-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57158-130">Optional query parameters</span></span>
<span data-ttu-id="57158-131">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57158-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57158-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57158-132">Request headers</span></span>
| <span data-ttu-id="57158-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57158-133">Header</span></span>       | <span data-ttu-id="57158-134">Значение</span><span class="sxs-lookup"><span data-stu-id="57158-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57158-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57158-135">Authorization</span></span>  | <span data-ttu-id="57158-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57158-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57158-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57158-138">Request body</span></span>
<span data-ttu-id="57158-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57158-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="57158-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="57158-140">Response</span></span>
<span data-ttu-id="57158-141">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [educationSubmission](../resources/educationsubmission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57158-141">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57158-142">Пример</span><span class="sxs-lookup"><span data-stu-id="57158-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57158-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="57158-143">Request</span></span>
<span data-ttu-id="57158-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57158-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57158-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="57158-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
# <a name="c"></a>[<span data-ttu-id="57158-146">C#</span><span class="sxs-lookup"><span data-stu-id="57158-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57158-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57158-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57158-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57158-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57158-149">Java</span><span class="sxs-lookup"><span data-stu-id="57158-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="57158-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="57158-150">Response</span></span>
<span data-ttu-id="57158-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="57158-151">The following is an example of the response.</span></span> 

><span data-ttu-id="57158-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57158-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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
