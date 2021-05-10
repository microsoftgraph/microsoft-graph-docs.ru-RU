---
title: Список унифицированныхRoleEligibilitySchedules
description: Получите список объектов unifiedRoleEligibilitySchedule и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d4a2c4ad3475b0f5a6a12f43248213cf3cf56af
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299511"
---
# <a name="list-unifiedroleeligibilityschedules"></a><span data-ttu-id="cfcd5-103">Список унифицированныхRoleEligibilitySchedules</span><span class="sxs-lookup"><span data-stu-id="cfcd5-103">List unifiedRoleEligibilitySchedules</span></span>
<span data-ttu-id="cfcd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfcd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfcd5-105">Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfcd5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcd5-106">Permissions</span></span>
<span data-ttu-id="cfcd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfcd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfcd5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcd5-109">Permission type</span></span>|<span data-ttu-id="cfcd5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfcd5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfcd5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfcd5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cfcd5-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cfcd5-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="cfcd5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfcd5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfcd5-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cfcd5-114">Not supported</span></span>|
|<span data-ttu-id="cfcd5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfcd5-115">Application</span></span>|<span data-ttu-id="cfcd5-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cfcd5-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfcd5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfcd5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfcd5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cfcd5-118">Optional query parameters</span></span>
<span data-ttu-id="cfcd5-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cfcd5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cfcd5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfcd5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfcd5-121">Request headers</span></span>
|<span data-ttu-id="cfcd5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cfcd5-122">Name</span></span>|<span data-ttu-id="cfcd5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cfcd5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cfcd5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfcd5-124">Authorization</span></span>|<span data-ttu-id="cfcd5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfcd5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfcd5-127">Request body</span></span>
<span data-ttu-id="cfcd5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfcd5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcd5-129">Response</span></span>

<span data-ttu-id="cfcd5-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfcd5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="cfcd5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfcd5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfcd5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules
```


### <a name="response"></a><span data-ttu-id="cfcd5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcd5-133">Response</span></span>
<span data-ttu-id="cfcd5-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cfcd5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "memberType": "direct"
    }
  ]
}
```

