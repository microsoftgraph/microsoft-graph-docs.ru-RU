---
title: 'accessPackageAssignment: filterByCurrentUser'
description: Извлечение списка объектов accesspackageassignment, фильтруемых на входе пользователя.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 72164fb7f9567d1a1c1b79316f19bbd304fabae3
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299550"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a><span data-ttu-id="ede95-103">accessPackageAssignment: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="ede95-103">accessPackageAssignment: filterByCurrentUser</span></span>
<span data-ttu-id="ede95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ede95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ede95-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)вы можете получить список объектов [accessPackageAssignment,](../resources/accesspackageassignment.md) фильтруемых для пользователя, входив в него.</span><span class="sxs-lookup"><span data-stu-id="ede95-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ede95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ede95-106">Permissions</span></span>
<span data-ttu-id="ede95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ede95-109">Permission type</span></span>|<span data-ttu-id="ede95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ede95-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ede95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ede95-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede95-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="ede95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ede95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede95-114">Not supported.</span></span>|
|<span data-ttu-id="ede95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ede95-115">Application</span></span>|<span data-ttu-id="ede95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ede95-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="ede95-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ede95-118">Function parameters</span></span>
<span data-ttu-id="ede95-119">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ede95-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ede95-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="ede95-120">Parameter</span></span>|<span data-ttu-id="ede95-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ede95-121">Type</span></span>|<span data-ttu-id="ede95-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ede95-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede95-123">on</span><span class="sxs-lookup"><span data-stu-id="ede95-123">on</span></span>|[<span data-ttu-id="ede95-124">accessPackageAssignmentFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="ede95-124">accessPackageAssignmentFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignment-accesspackageassignmentfilterbycurrentuseroptions.md)|<span data-ttu-id="ede95-125">Список текущих пользовательских параметров, которые можно использовать для фильтрации в списке назначений пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="ede95-125">The list of current user options that can be used to filter on the access package assignments list.</span></span>|

- <span data-ttu-id="ede95-126">`target` используется для получения объектов, в которых целевым объектом является пользователь, заявив `accessPackageAssignment` о подписании.</span><span class="sxs-lookup"><span data-stu-id="ede95-126">`target` is used to get the `accessPackageAssignment` objects where the signed-in user is the target.</span></span> <span data-ttu-id="ede95-127">В итоговом списке содержатся все назначения, текущие и просроченные, для вызываемого во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="ede95-127">The resulting list includes all of the assignments, current and expired, for the caller across all catalogs and access packages.</span></span>

- <span data-ttu-id="ede95-128">`createdBy` используется для получения `accessPackageAssignment` объектов, созданных подписанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="ede95-128">`createdBy` is used to get the `accessPackageAssignment` objects created by the signed-in user.</span></span> <span data-ttu-id="ede95-129">В итоговом списке содержатся все назначения, созданные вызываемой для себя или от имени других лиц, например в случае прямого назначения администратора, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="ede95-129">The resulting list includes all of the assignments that the caller created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ede95-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ede95-130">Request headers</span></span>
|<span data-ttu-id="ede95-131">Имя</span><span class="sxs-lookup"><span data-stu-id="ede95-131">Name</span></span>|<span data-ttu-id="ede95-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ede95-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ede95-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ede95-133">Authorization</span></span>|<span data-ttu-id="ede95-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ede95-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede95-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ede95-136">Request body</span></span>
<span data-ttu-id="ede95-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ede95-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ede95-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede95-138">Response</span></span>

<span data-ttu-id="ede95-139">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [коллекцию accessPackageAssignment](../resources/accesspackageassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ede95-139">If successful, this method returns a `200 OK` response code and an [accessPackageAssignment](../resources/accesspackageassignment.md) collection in the response body.</span></span>

<span data-ttu-id="ede95-140">Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством в ответе, содержам URL-адрес на `@odata.nextLink` следующую страницу результатов.</span><span class="sxs-lookup"><span data-stu-id="ede95-140">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="ede95-141">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом в каждом ответе, пока не будут возвращены `@odata.nextLink` все результаты.</span><span class="sxs-lookup"><span data-stu-id="ede95-141">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned.</span></span> <span data-ttu-id="ede95-142">Дополнительные сведения см. [в Graph microsoft Graph в приложении.](/graph/paging.md)</span><span class="sxs-lookup"><span data-stu-id="ede95-142">For more information, see [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

## <a name="examples"></a><span data-ttu-id="ede95-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="ede95-143">Examples</span></span>

<span data-ttu-id="ede95-144">В следующем примере получается состояние назначений пакетов доступа, целевых для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ede95-144">The following example gets the status of access package assignments targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="ede95-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ede95-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')
```


### <a name="response"></a><span data-ttu-id="ede95-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede95-146">Response</span></span>
> <span data-ttu-id="ede95-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ede95-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
            "catalogId": "34cfe9a8-88bc-4c82-b3d8-6b77d7035c33",
            "accessPackageId": "ca6992f8-e413-49a1-9619-c9819f4f73e0",
            "assignmentPolicyId": "7c6e6874-789e-4f11-b351-cc7b5883deef",
            "targetId": "2cb14f51-0108-41d8-89da-cd0e05e2c988",
            "assignmentStatus": "Delivered",
            "assignmentState": "Delivered",
            "isExtended": false,
            "expiredDateTime": null,
            "schedule": {
                "startDateTime": "2021-01-19T20:02:36.013Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": "2022-01-19T20:02:36.013Z",
                    "duration": null,
                    "type": "afterDateTime"
                }
            }
        }
  ]
}

```

