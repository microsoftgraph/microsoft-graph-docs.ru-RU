---
title: Get educationAssignmentSettings
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fbc7a5c17c0d980de9baa95d625d7bb058b167e9
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912697"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="003f8-103">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="003f8-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="003f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="003f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="003f8-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="003f8-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="003f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="003f8-106">Permissions</span></span>
<span data-ttu-id="003f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="003f8-109">Permission type</span></span>|<span data-ttu-id="003f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="003f8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="003f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="003f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="003f8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003f8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="003f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="003f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="003f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="003f8-114">Not supported.</span></span>|
|<span data-ttu-id="003f8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="003f8-115">Application</span></span>| <span data-ttu-id="003f8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003f8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="003f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="003f8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="003f8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="003f8-118">Optional query parameters</span></span>
<span data-ttu-id="003f8-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="003f8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="003f8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="003f8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="003f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="003f8-121">Request headers</span></span>
|<span data-ttu-id="003f8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="003f8-122">Name</span></span>|<span data-ttu-id="003f8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="003f8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="003f8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="003f8-124">Authorization</span></span>|<span data-ttu-id="003f8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="003f8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="003f8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="003f8-127">Request body</span></span>
<span data-ttu-id="003f8-128">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="003f8-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="003f8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="003f8-129">Response</span></span>

<span data-ttu-id="003f8-130">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="003f8-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="003f8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="003f8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="003f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="003f8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

### <a name="response"></a><span data-ttu-id="003f8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="003f8-133">Response</span></span>
<span data-ttu-id="003f8-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="003f8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

