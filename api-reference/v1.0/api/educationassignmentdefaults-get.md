---
title: Get educationAssignmentDefaults
description: Ознакомьтесь с свойствами и отношениями объекта educationAssignmentDefaults.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 190099048769ed0a45a8279db35a40bdbf04b612
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912919"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="85be6-103">Get educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="85be6-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="85be6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85be6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85be6-105">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="85be6-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> 

<span data-ttu-id="85be6-106">Это по умолчанию назначения класса, которые соблюдаются новыми назначениями, созданными в классе.</span><span class="sxs-lookup"><span data-stu-id="85be6-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="85be6-107">Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="85be6-107">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="85be6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85be6-108">Permissions</span></span>
<span data-ttu-id="85be6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85be6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85be6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85be6-111">Permission type</span></span>|<span data-ttu-id="85be6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85be6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85be6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85be6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="85be6-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85be6-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="85be6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85be6-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="85be6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85be6-116">Not supported.</span></span> |
|<span data-ttu-id="85be6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="85be6-117">Application</span></span>| <span data-ttu-id="85be6-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85be6-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85be6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85be6-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85be6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85be6-120">Optional query parameters</span></span>
<span data-ttu-id="85be6-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="85be6-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="85be6-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="85be6-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="85be6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85be6-123">Request headers</span></span>
|<span data-ttu-id="85be6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="85be6-124">Name</span></span>|<span data-ttu-id="85be6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="85be6-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85be6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85be6-126">Authorization</span></span>|<span data-ttu-id="85be6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85be6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85be6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85be6-129">Request body</span></span>
<span data-ttu-id="85be6-130">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85be6-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85be6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85be6-131">Response</span></span>

<span data-ttu-id="85be6-132">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="85be6-132">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85be6-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="85be6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85be6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="85be6-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

### <a name="response"></a><span data-ttu-id="85be6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="85be6-135">Response</span></span>
<span data-ttu-id="85be6-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85be6-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('c6f4e171-da1f-4598-a648-05fcec6cd9ba')"
  }
}
```

