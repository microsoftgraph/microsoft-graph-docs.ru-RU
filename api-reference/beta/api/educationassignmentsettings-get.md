---
title: Get educationAssignmentSettings
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5f383ee9cfbb4824990b0c7c49da7852cbeb055
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061667"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="220c1-103">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="220c1-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="220c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="220c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="220c1-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="220c1-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="220c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="220c1-106">Permissions</span></span>
<span data-ttu-id="220c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="220c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="220c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="220c1-109">Permission type</span></span>|<span data-ttu-id="220c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="220c1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="220c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="220c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="220c1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="220c1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="220c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="220c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="220c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="220c1-114">Not supported.</span></span>|
|<span data-ttu-id="220c1-115">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="220c1-115">Application\*</span></span>| <span data-ttu-id="220c1-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="220c1-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="220c1-117">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="220c1-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="220c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="220c1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="220c1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="220c1-119">Optional query parameters</span></span>
<span data-ttu-id="220c1-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="220c1-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="220c1-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="220c1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="220c1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="220c1-122">Request headers</span></span>
|<span data-ttu-id="220c1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="220c1-123">Name</span></span>|<span data-ttu-id="220c1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="220c1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="220c1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="220c1-125">Authorization</span></span>|<span data-ttu-id="220c1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="220c1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="220c1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="220c1-128">Request body</span></span>
<span data-ttu-id="220c1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="220c1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="220c1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="220c1-130">Response</span></span>

<span data-ttu-id="220c1-131">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="220c1-131">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="220c1-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="220c1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="220c1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="220c1-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="220c1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="220c1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="220c1-135">C#</span><span class="sxs-lookup"><span data-stu-id="220c1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220c1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220c1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220c1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220c1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="220c1-138">Java</span><span class="sxs-lookup"><span data-stu-id="220c1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="220c1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="220c1-139">Response</span></span>
<span data-ttu-id="220c1-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="220c1-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

