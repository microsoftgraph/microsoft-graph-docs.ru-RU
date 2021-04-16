---
title: действие createCopy
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 353c55305eb0a09cdf26beecf1cf5e222338af3b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869089"
---
# <a name="createcopy-action"></a><span data-ttu-id="5df50-103">действие createCopy</span><span class="sxs-lookup"><span data-stu-id="5df50-103">createCopy action</span></span>

<span data-ttu-id="5df50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5df50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5df50-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5df50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df50-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5df50-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5df50-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5df50-108">Prerequisites</span></span>
<span data-ttu-id="5df50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5df50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5df50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5df50-111">Permission type</span></span>|<span data-ttu-id="5df50-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5df50-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5df50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5df50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5df50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5df50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5df50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5df50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df50-116">Not supported.</span></span>|
|<span data-ttu-id="5df50-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="5df50-117">Application</span></span>|<span data-ttu-id="5df50-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df50-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5df50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5df50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="5df50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5df50-120">Request headers</span></span>
|<span data-ttu-id="5df50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5df50-121">Header</span></span>|<span data-ttu-id="5df50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5df50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5df50-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5df50-123">Authorization</span></span>|<span data-ttu-id="5df50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5df50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5df50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5df50-125">Accept</span></span>|<span data-ttu-id="5df50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5df50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5df50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5df50-127">Request body</span></span>
<span data-ttu-id="5df50-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5df50-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5df50-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5df50-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5df50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5df50-130">Property</span></span>|<span data-ttu-id="5df50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5df50-131">Type</span></span>|<span data-ttu-id="5df50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5df50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df50-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5df50-133">displayName</span></span>|<span data-ttu-id="5df50-134">String</span><span class="sxs-lookup"><span data-stu-id="5df50-134">String</span></span>|<span data-ttu-id="5df50-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5df50-135">Not yet documented</span></span>|
|<span data-ttu-id="5df50-136">description</span><span class="sxs-lookup"><span data-stu-id="5df50-136">description</span></span>|<span data-ttu-id="5df50-137">String</span><span class="sxs-lookup"><span data-stu-id="5df50-137">String</span></span>|<span data-ttu-id="5df50-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5df50-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5df50-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5df50-139">Response</span></span>
<span data-ttu-id="5df50-140">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [устройствоManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5df50-140">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5df50-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5df50-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5df50-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5df50-142">Request</span></span>
<span data-ttu-id="5df50-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5df50-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy

Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="5df50-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5df50-144">Response</span></span>
<span data-ttu-id="5df50-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5df50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
    "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
    "name": "Name value",
    "description": "Description value",
    "platforms": "macOS",
    "technologies": "mdm",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "settingCount": 12,
    "creationSource": "Creation Source value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "isAssigned": true,
    "templateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
      "templateId": "Template Id value",
      "templateFamily": "endpointSecurityAntivirus",
      "templateDisplayName": "Template Display Name value",
      "templateDisplayVersion": "Template Display Version value"
    }
  }
}
```




