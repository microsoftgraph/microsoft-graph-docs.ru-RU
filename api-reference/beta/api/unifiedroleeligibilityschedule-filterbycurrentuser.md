---
title: 'unifiedRoleEligibilitySchedule: filterByCurrentUser'
description: Получите список объектов unifiedRoleEligibilitySchedule и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c74306e5e39200db1dd5b0ede2a93a818e928f11
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334712"
---
# <a name="unifiedroleeligibilityschedule-filterbycurrentuser"></a><span data-ttu-id="9f31f-103">unifiedRoleEligibilitySchedule: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="9f31f-103">unifiedRoleEligibilitySchedule: filterByCurrentUser</span></span>
<span data-ttu-id="9f31f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f31f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f31f-105">Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) и их свойств, связанных с определенным основным объектом.</span><span class="sxs-lookup"><span data-stu-id="9f31f-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f31f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f31f-106">Permissions</span></span>
<span data-ttu-id="9f31f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f31f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f31f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f31f-109">Permission type</span></span>|<span data-ttu-id="9f31f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f31f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f31f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f31f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f31f-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9f31f-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="9f31f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f31f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f31f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9f31f-114">Not supported</span></span>|
|<span data-ttu-id="9f31f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f31f-115">Application</span></span>|<span data-ttu-id="9f31f-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9f31f-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f31f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f31f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="9f31f-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="9f31f-118">Query parameters</span></span>
<span data-ttu-id="9f31f-119">В следующей таблице показаны параметры, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f31f-119">The following table shows the parameters that can be used with this method.</span></span>

|<span data-ttu-id="9f31f-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f31f-120">Parameter</span></span>|<span data-ttu-id="9f31f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9f31f-121">Type</span></span>|<span data-ttu-id="9f31f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9f31f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f31f-123">on</span><span class="sxs-lookup"><span data-stu-id="9f31f-123">on</span></span>|<span data-ttu-id="9f31f-124">roleEligibilityScheduleFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="9f31f-124">roleEligibilityScheduleFilterByCurrentUserOptions</span></span>|<span data-ttu-id="9f31f-125">Id текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f31f-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="9f31f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f31f-126">Request headers</span></span>
|<span data-ttu-id="9f31f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="9f31f-127">Name</span></span>|<span data-ttu-id="9f31f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9f31f-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f31f-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f31f-129">Authorization</span></span>|<span data-ttu-id="9f31f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f31f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f31f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f31f-132">Request body</span></span>
<span data-ttu-id="9f31f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f31f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f31f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f31f-134">Response</span></span>

<span data-ttu-id="9f31f-135">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f31f-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f31f-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f31f-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f31f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f31f-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='eb18c026-c026-eb18-26c0-18eb26c018eb')
```


### <a name="response"></a><span data-ttu-id="9f31f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f31f-138">Response</span></span>
<span data-ttu-id="9f31f-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f31f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "createdUsing": "eb18c026-c026-eb18-26c0-18eb26c018eb",
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

