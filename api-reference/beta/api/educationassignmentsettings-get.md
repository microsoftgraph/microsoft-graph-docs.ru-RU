---
title: Get educationAssignmentSettings
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e65a154b17a1b7e1491908b03a5125bc69006fcd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773636"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="142c3-103">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="142c3-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="142c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="142c3-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="142c3-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="142c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="142c3-106">Permissions</span></span>
<span data-ttu-id="142c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="142c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="142c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="142c3-109">Permission type</span></span>|<span data-ttu-id="142c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="142c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="142c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="142c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="142c3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="142c3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="142c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="142c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="142c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142c3-114">Not supported.</span></span>|
|<span data-ttu-id="142c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="142c3-115">Application</span></span>|<span data-ttu-id="142c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="142c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="142c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="142c3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="142c3-118">Optional query parameters</span></span>
<span data-ttu-id="142c3-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="142c3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="142c3-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="142c3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="142c3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="142c3-121">Request headers</span></span>
|<span data-ttu-id="142c3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="142c3-122">Name</span></span>|<span data-ttu-id="142c3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="142c3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="142c3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="142c3-124">Authorization</span></span>|<span data-ttu-id="142c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="142c3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="142c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="142c3-127">Request body</span></span>
<span data-ttu-id="142c3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="142c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="142c3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="142c3-129">Response</span></span>

<span data-ttu-id="142c3-130">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="142c3-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="142c3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="142c3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="142c3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="142c3-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="142c3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="142c3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="142c3-134">C#</span><span class="sxs-lookup"><span data-stu-id="142c3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="142c3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="142c3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="142c3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="142c3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="142c3-137">Java</span><span class="sxs-lookup"><span data-stu-id="142c3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="142c3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="142c3-138">Response</span></span>
<span data-ttu-id="142c3-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="142c3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

