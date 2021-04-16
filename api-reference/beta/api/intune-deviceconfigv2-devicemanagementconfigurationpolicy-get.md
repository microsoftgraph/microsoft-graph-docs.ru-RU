---
title: Get deviceManagementConfigurationPolicy
description: Чтение свойств и связей объекта deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30a20e96306752ff6b9fcda56d7f738a5056d90a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867100"
---
# <a name="get-devicemanagementconfigurationpolicy"></a><span data-ttu-id="93329-103">Get deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="93329-103">Get deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="93329-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93329-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93329-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93329-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93329-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93329-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93329-107">Чтение свойств и связей [объекта deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93329-107">Read properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93329-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93329-108">Prerequisites</span></span>
<span data-ttu-id="93329-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93329-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93329-111">Permission type</span></span>|<span data-ttu-id="93329-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93329-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93329-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93329-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93329-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93329-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93329-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93329-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93329-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93329-116">Not supported.</span></span>|
|<span data-ttu-id="93329-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="93329-117">Application</span></span>|<span data-ttu-id="93329-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93329-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93329-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93329-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
GET /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93329-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93329-120">Optional query parameters</span></span>
<span data-ttu-id="93329-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93329-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93329-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93329-122">Request headers</span></span>
|<span data-ttu-id="93329-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93329-123">Header</span></span>|<span data-ttu-id="93329-124">Значение</span><span class="sxs-lookup"><span data-stu-id="93329-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93329-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93329-125">Authorization</span></span>|<span data-ttu-id="93329-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93329-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93329-127">Accept</span><span class="sxs-lookup"><span data-stu-id="93329-127">Accept</span></span>|<span data-ttu-id="93329-128">application/json</span><span class="sxs-lookup"><span data-stu-id="93329-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93329-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93329-129">Request body</span></span>
<span data-ttu-id="93329-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93329-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93329-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="93329-131">Response</span></span>
<span data-ttu-id="93329-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93329-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93329-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93329-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="93329-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="93329-134">Request</span></span>
<span data-ttu-id="93329-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93329-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
```

### <a name="response"></a><span data-ttu-id="93329-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93329-136">Response</span></span>
<span data-ttu-id="93329-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93329-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




