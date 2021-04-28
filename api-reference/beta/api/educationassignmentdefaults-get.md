---
title: Get educationAssignmentDefaults
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentDefaults.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 74840c4ac794262d7e5b7cced90c535e5132aa18
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061702"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="0e55a-103">Get educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="0e55a-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="0e55a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e55a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e55a-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="0e55a-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="0e55a-106">Это по умолчанию назначения класса, которые соблюдаются новыми назначениями, созданными в классе.</span><span class="sxs-lookup"><span data-stu-id="0e55a-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="0e55a-107">Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0e55a-107">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e55a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e55a-108">Permissions</span></span>
<span data-ttu-id="0e55a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e55a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e55a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e55a-111">Permission type</span></span>|<span data-ttu-id="0e55a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e55a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e55a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e55a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0e55a-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e55a-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="0e55a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e55a-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0e55a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e55a-116">Not supported.</span></span> |
|<span data-ttu-id="0e55a-117">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="0e55a-117">Application\*</span></span>| <span data-ttu-id="0e55a-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e55a-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="0e55a-119">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="0e55a-119">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="0e55a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e55a-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e55a-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e55a-121">Optional query parameters</span></span>
<span data-ttu-id="0e55a-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0e55a-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e55a-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0e55a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e55a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e55a-124">Request headers</span></span>
|<span data-ttu-id="0e55a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0e55a-125">Name</span></span>|<span data-ttu-id="0e55a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0e55a-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e55a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e55a-127">Authorization</span></span>|<span data-ttu-id="0e55a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e55a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e55a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e55a-130">Request body</span></span>
<span data-ttu-id="0e55a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e55a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e55a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e55a-132">Response</span></span>

<span data-ttu-id="0e55a-133">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0e55a-133">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e55a-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e55a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e55a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e55a-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0e55a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e55a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
```
# <a name="c"></a>[<span data-ttu-id="0e55a-137">C#</span><span class="sxs-lookup"><span data-stu-id="0e55a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e55a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e55a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e55a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e55a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e55a-140">Java</span><span class="sxs-lookup"><span data-stu-id="0e55a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0e55a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e55a-141">Response</span></span>
<span data-ttu-id="0e55a-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e55a-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

