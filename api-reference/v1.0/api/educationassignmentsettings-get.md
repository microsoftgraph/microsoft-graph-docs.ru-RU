---
title: Get educationAssignmentSettings
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c2758258126203ff8099dc5a162ade00a32ffb4
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993520"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="55478-103">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="55478-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="55478-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55478-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55478-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="55478-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55478-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55478-106">Permissions</span></span>
<span data-ttu-id="55478-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55478-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55478-109">Permission type</span></span>|<span data-ttu-id="55478-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55478-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55478-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55478-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55478-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55478-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="55478-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55478-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55478-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55478-114">Not supported.</span></span>|
|<span data-ttu-id="55478-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="55478-115">Application</span></span>| <span data-ttu-id="55478-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55478-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55478-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55478-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55478-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55478-118">Optional query parameters</span></span>
<span data-ttu-id="55478-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="55478-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="55478-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55478-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55478-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55478-121">Request headers</span></span>
|<span data-ttu-id="55478-122">Имя</span><span class="sxs-lookup"><span data-stu-id="55478-122">Name</span></span>|<span data-ttu-id="55478-123">Описание</span><span class="sxs-lookup"><span data-stu-id="55478-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55478-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55478-124">Authorization</span></span>|<span data-ttu-id="55478-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55478-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55478-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55478-127">Request body</span></span>
<span data-ttu-id="55478-128">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55478-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55478-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="55478-129">Response</span></span>

<span data-ttu-id="55478-130">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55478-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55478-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="55478-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55478-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="55478-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="55478-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55478-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="55478-134">C#</span><span class="sxs-lookup"><span data-stu-id="55478-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55478-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55478-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55478-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55478-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55478-137">Java</span><span class="sxs-lookup"><span data-stu-id="55478-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55478-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="55478-138">Response</span></span>
<span data-ttu-id="55478-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55478-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "submissionAnimationDisabled": false
  }
}
```

