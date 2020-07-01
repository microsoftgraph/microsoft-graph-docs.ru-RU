---
title: 'Синчронизатионжоб: Провисионондеманд'
description: Выберите пользователя и подготовьте учетную запись по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b333350b335e431808caa74f65dc1f61601cddb
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007211"
---
# <a name="synchronizationjob-provisionondemand"></a><span data-ttu-id="a1bf7-103">Синчронизатионжоб: Провисионондеманд</span><span class="sxs-lookup"><span data-stu-id="a1bf7-103">synchronizationJob: provisionOnDemand</span></span>

<span data-ttu-id="a1bf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1bf7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1bf7-105">Выберите пользователя и подготовьте учетную запись по требованию.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-105">Select a user and provision the account on-demand.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1bf7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1bf7-106">Permissions</span></span>
<span data-ttu-id="a1bf7-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a1bf7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1bf7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1bf7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1bf7-109">Permission type</span></span>                        | <span data-ttu-id="a1bf7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1bf7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1bf7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1bf7-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="a1bf7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1bf7-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a1bf7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1bf7-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a1bf7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-114">Not supported.</span></span> |
|<span data-ttu-id="a1bf7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1bf7-115">Application</span></span>                            |<span data-ttu-id="a1bf7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a1bf7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1bf7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
```

## <a name="request-headers"></a><span data-ttu-id="a1bf7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1bf7-118">Request headers</span></span>
|<span data-ttu-id="a1bf7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a1bf7-119">Name</span></span>|<span data-ttu-id="a1bf7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a1bf7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a1bf7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1bf7-121">Authorization</span></span>|<span data-ttu-id="a1bf7-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-122">Bearer {token}.</span></span> <span data-ttu-id="a1bf7-123">Required.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-123">Required.</span></span>|
|<span data-ttu-id="a1bf7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1bf7-124">Content-Type</span></span>|<span data-ttu-id="a1bf7-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-125">application/json.</span></span> <span data-ttu-id="a1bf7-126">Required.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1bf7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1bf7-127">Request body</span></span>
<span data-ttu-id="a1bf7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a1bf7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a1bf7-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a1bf7-130">Parameter</span></span>|<span data-ttu-id="a1bf7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a1bf7-131">Type</span></span>|<span data-ttu-id="a1bf7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a1bf7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1bf7-133">parameters</span><span class="sxs-lookup"><span data-stu-id="a1bf7-133">parameters</span></span>|<span data-ttu-id="a1bf7-134">Коллекция [синчронизатионжобаппликатионпараметерс](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="a1bf7-134">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="a1bf7-135">Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-135">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="a1bf7-136">Ресурс в основном используется для подготовки по требованию.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-136">The resource is primarily used for on-demand provisioning.</span></span> |



## <a name="response"></a><span data-ttu-id="a1bf7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1bf7-137">Response</span></span>

<span data-ttu-id="a1bf7-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект стрингкэйстрингвалуепаир.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-138">If successful, this method returns a `200 OK` response code and a stringKeyStringValuePair.</span></span>

## <a name="examples"></a><span data-ttu-id="a1bf7-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a1bf7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1bf7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1bf7-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand

Content-Type: application/json
Content-length: 122

{
    "parameters" [{
      "subjects": [{
          "objectId": "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          "objectType": "User"
      }],
      "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  }
```


### <a name="response"></a><span data-ttu-id="a1bf7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1bf7-141">Response</span></span>
<span data-ttu-id="a1bf7-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1bf7-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
``` 
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.stringKeyStringValuePair",
    "key": "{\"result\":\"Skipped\",\"details\":{\"errorCode\":\"RedundantExport\",\"errorMessage\":\"The state of the user in both the source and target systems already match.\"}}",
    "value": "{\"action\":\"Other\",\"changeId\":\"g8ba3be8-1d7f-4a60-ae31-a8980da0a389\",\"endTime\":\"2020-06-26T13:58:24.7682084Z\",\"modifiedProperties\":[{\"displayName\":\"objectId\",\"oldValue\":null,\"newValue\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\"},{\"displayName\":\"accountEnabled\",\"oldValue\":null,\"newValue\":\"True\"},{\"displayName\":\"displayName\",\"oldValue\":null,\"newValue\":\"Bill Bob\"},{\"displayName\":\"mailNickname\",\"oldValue\":null,\"newValue\":\"Bill\"},{\"displayName\":\"userPrincipalName\",\"oldValue\":null,\"newValue\":\"BillBob@scimreftest.onmicrosoft.com\"},{\"displayName\":\"IsSoftDeleted\",\"oldValue\":null,\"newValue\":\"False\"},{\"displayName\":\"appRoleAssignments\",\"oldValue\":null,\"newValue\":\"User\"}],\"provisioningSteps\":[{\"name\":\"EntryImport\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Retrieved User 'BillBob@scimreftest.onmicrosoft.com' from Azure Active Directory\",\"timestamp\":\"2020-06-26T13:58:24.5494971Z\",\"details\":{\"objectId\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\",\"accountEnabled\":\"True\",\"displayName\":\"Fill Bob\",\"mailNickname\":\"Bill\",\"userPrincipalName\":\"BillBob@scimreftest.onmicrosoft.com\",\"IsSoftDeleted\":\"False\",\"appRoleAssignments\":\"User\"}},{\"name\":\"EntryImport\",\"type\":\"Matching\",\"status\":\"Success\",\"description\":\"Retrieved  'BillBob@scimreftest.onmicrosoft.com' from customappsso\",\"timestamp\":\"2020-06-26T13:58:24.7214072Z\",\"details\":{\"active\":\"True\",\"displayName\":\"Bill Bob\",\"externalId\":\"Bill\",\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"userName\":\"BillBob@scimreftest.onmicrosoft.com\"}},{\"name\":\"EntrySynchronizationScoping\",\"type\":\"Scoping\",\"status\":\"Success\",\"description\":\"Determine if User in scope by evaluating against each scoping filter\",\"timestamp\":\"2020-06-26T13:58:24.7526181Z\",\"details\":{\"IsActive\":\"True\",\"Assigned\":\"True\",\"IsEffectivelyEntitledForProvisioning\":\"True\",\"IsInProvisioningScopeDisplayName\":\"True\",\"ScopeEvaluationResult\":\"{}\"}},{\"name\":\"EntrySynchronizationSkip\",\"type\":\"Export\",\"status\":\"Skipped\",\"description\":\"The state of the user in both the source and target systems already match. No change to the User 'BillBob@scimreftest.onmicrosoft.com' currently needs to be made.\",\"timestamp\":\"2020-06-26T13:58:24.7682084Z\",\"details\":{\"SkipReason\":\"RedundantExport\"}}],\"reportableIdentifier\":\"BillBob@scimreftest.onmicrosoft.com\",\"startTime\":\"2020-06-26T13:58:24.5494971Z\",\"statusInfo\":{\"status\":\"Skipped\",\"errorCode\":null,\"reason\":null,\"additionalDetails\":null,\"errorCategory\":null,\"recommendedAction\":null},\"sourceIdentity\":{\"id\":\"62cf7b7a-52be-4a9b-9c69-e5d4a4a14f67\",\"type\":\"User\",\"displayName\":null,\"details\":null},\"sourceSystem\":{\"id\":null,\"name\":\"Azure Active Directory\",\"details\":null},\"targetIdentity\":{\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"type\":\"urn:ietf:params:scim:schemas:extension:enterprise:2.0:User\",\"displayName\":null,\"details\":null},\"targetSystem\":{\"id\":null,\"name\":\"customappsso\",\"details\":null}}"
}
```
