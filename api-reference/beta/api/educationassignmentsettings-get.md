---
title: Get educationAssignmentSettings
description: Чтение свойств и связей объекта educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 896e47bded7ee5d34a2b923107737feafbf37144
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034354"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="64723-103">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="64723-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="64723-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64723-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64723-105">Чтение свойств и связей объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="64723-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64723-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64723-106">Permissions</span></span>
<span data-ttu-id="64723-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64723-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64723-109">Permission type</span></span>|<span data-ttu-id="64723-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64723-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64723-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64723-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64723-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64723-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="64723-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64723-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64723-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64723-114">Not supported.</span></span>|
|<span data-ttu-id="64723-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64723-115">Application</span></span>|<span data-ttu-id="64723-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64723-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64723-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64723-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64723-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64723-118">Optional query parameters</span></span>
<span data-ttu-id="64723-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="64723-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64723-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="64723-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64723-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64723-121">Request headers</span></span>
|<span data-ttu-id="64723-122">Имя</span><span class="sxs-lookup"><span data-stu-id="64723-122">Name</span></span>|<span data-ttu-id="64723-123">Описание</span><span class="sxs-lookup"><span data-stu-id="64723-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64723-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64723-124">Authorization</span></span>|<span data-ttu-id="64723-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64723-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64723-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64723-127">Request body</span></span>
<span data-ttu-id="64723-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64723-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64723-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="64723-129">Response</span></span>

<span data-ttu-id="64723-130">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64723-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64723-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="64723-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64723-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="64723-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```

### <a name="response"></a><span data-ttu-id="64723-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64723-133">Response</span></span>
<span data-ttu-id="64723-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64723-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

