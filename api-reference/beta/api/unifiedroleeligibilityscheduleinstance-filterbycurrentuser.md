---
title: 'unifiedRoleEligibilityScheduleInstance: filterByCurrentUser'
description: Получите список объектов unifiedRoleEligibilityScheduleInstance и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 724933c90a7a404b360e19a76304ba1d99be25bb
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679913"
---
# <a name="unifiedroleeligibilityscheduleinstance-filterbycurrentuser"></a><span data-ttu-id="0e61b-103">unifiedRoleEligibilityScheduleInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="0e61b-103">unifiedRoleEligibilityScheduleInstance: filterByCurrentUser</span></span>
<span data-ttu-id="0e61b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e61b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e61b-105">Получите список объектов [unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) и их свойств, связанных с определенным основным объектом.</span><span class="sxs-lookup"><span data-stu-id="0e61b-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e61b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e61b-106">Permissions</span></span>
<span data-ttu-id="0e61b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e61b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e61b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e61b-109">Permission type</span></span>|<span data-ttu-id="0e61b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e61b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e61b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e61b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e61b-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0e61b-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="0e61b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e61b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e61b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0e61b-114">Not supported</span></span>|
|<span data-ttu-id="0e61b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e61b-115">Application</span></span>|<span data-ttu-id="0e61b-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0e61b-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e61b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e61b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="0e61b-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="0e61b-118">Query parameters</span></span>
<span data-ttu-id="0e61b-119">В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e61b-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="0e61b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="0e61b-120">Parameter</span></span>|<span data-ttu-id="0e61b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0e61b-121">Type</span></span>|<span data-ttu-id="0e61b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0e61b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e61b-123">on</span><span class="sxs-lookup"><span data-stu-id="0e61b-123">on</span></span>|<span data-ttu-id="0e61b-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="0e61b-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span></span>|<span data-ttu-id="0e61b-125">Id текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e61b-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="0e61b-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e61b-126">Request headers</span></span>
|<span data-ttu-id="0e61b-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0e61b-127">Name</span></span>|<span data-ttu-id="0e61b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0e61b-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e61b-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e61b-129">Authorization</span></span>|<span data-ttu-id="0e61b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e61b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e61b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e61b-132">Request body</span></span>
<span data-ttu-id="0e61b-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e61b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e61b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e61b-134">Response</span></span>

<span data-ttu-id="0e61b-135">В случае успешной работы этот метод возвращает код ответа и `200 OK` [унифицированную коллекциюRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0e61b-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e61b-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e61b-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e61b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e61b-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser(on='5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
```


### <a name="response"></a><span data-ttu-id="0e61b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e61b-138">Response</span></span>
<span data-ttu-id="0e61b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e61b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
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
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c"
    }
  ]
}
```

