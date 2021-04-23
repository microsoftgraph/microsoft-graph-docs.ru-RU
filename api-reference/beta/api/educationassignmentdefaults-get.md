---
title: Get educationAssignmentDefaults
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentDefaults.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 863ff034080250fc7ce4cfc5b22344fcd2374fad
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961298"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="75f4d-103">Get educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="75f4d-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="75f4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f4d-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="75f4d-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="75f4d-106">Это по умолчанию назначения класса, которые соблюдаются новыми назначениями, созданными в классе.</span><span class="sxs-lookup"><span data-stu-id="75f4d-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="75f4d-107">Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="75f4d-107">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="75f4d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75f4d-108">Permissions</span></span>
<span data-ttu-id="75f4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75f4d-111">Permission type</span></span>|<span data-ttu-id="75f4d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75f4d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f4d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="75f4d-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75f4d-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="75f4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f4d-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="75f4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f4d-116">Not supported.</span></span> |
|<span data-ttu-id="75f4d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75f4d-117">Application</span></span>| <span data-ttu-id="75f4d-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75f4d-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="75f4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f4d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75f4d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75f4d-120">Optional query parameters</span></span>
<span data-ttu-id="75f4d-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="75f4d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="75f4d-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75f4d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75f4d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f4d-123">Request headers</span></span>
|<span data-ttu-id="75f4d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="75f4d-124">Name</span></span>|<span data-ttu-id="75f4d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="75f4d-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75f4d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f4d-126">Authorization</span></span>|<span data-ttu-id="75f4d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75f4d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f4d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75f4d-129">Request body</span></span>
<span data-ttu-id="75f4d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75f4d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f4d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f4d-131">Response</span></span>

<span data-ttu-id="75f4d-132">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75f4d-132">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75f4d-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="75f4d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75f4d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f4d-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="75f4d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f4d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
```
# <a name="c"></a>[<span data-ttu-id="75f4d-136">C#</span><span class="sxs-lookup"><span data-stu-id="75f4d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f4d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f4d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f4d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f4d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f4d-139">Java</span><span class="sxs-lookup"><span data-stu-id="75f4d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="75f4d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f4d-140">Response</span></span>
<span data-ttu-id="75f4d-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75f4d-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "addedStudentAction": "none",
    "dueTime": "23:59:00",
    "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
  }
}
```

