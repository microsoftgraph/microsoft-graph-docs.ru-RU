---
title: Get deviceManagementConfigurationPolicyTemplate
description: Чтение свойств и связей объекта deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a255f909f6f49db7a618c006a51acd5f1c803f5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665888"
---
# <a name="get-devicemanagementconfigurationpolicytemplate"></a><span data-ttu-id="eaa54-103">Get deviceManagementConfigurationPolicyTemplate</span><span class="sxs-lookup"><span data-stu-id="eaa54-103">Get deviceManagementConfigurationPolicyTemplate</span></span>

<span data-ttu-id="eaa54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaa54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaa54-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaa54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaa54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaa54-107">Чтение свойств и связей [объекта deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)</span><span class="sxs-lookup"><span data-stu-id="eaa54-107">Read properties and relationships of the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaa54-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eaa54-108">Prerequisites</span></span>
<span data-ttu-id="eaa54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaa54-111">Permission type</span></span>|<span data-ttu-id="eaa54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaa54-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaa54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaa54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaa54-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa54-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eaa54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaa54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaa54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa54-116">Not supported.</span></span>|
|<span data-ttu-id="eaa54-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="eaa54-117">Application</span></span>|<span data-ttu-id="eaa54-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa54-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaa54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaa54-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eaa54-120">Optional query parameters</span></span>
<span data-ttu-id="eaa54-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eaa54-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaa54-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaa54-122">Request headers</span></span>
|<span data-ttu-id="eaa54-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaa54-123">Header</span></span>|<span data-ttu-id="eaa54-124">Значение</span><span class="sxs-lookup"><span data-stu-id="eaa54-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaa54-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa54-125">Authorization</span></span>|<span data-ttu-id="eaa54-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaa54-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaa54-127">Accept</span><span class="sxs-lookup"><span data-stu-id="eaa54-127">Accept</span></span>|<span data-ttu-id="eaa54-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eaa54-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaa54-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaa54-129">Request body</span></span>
<span data-ttu-id="eaa54-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaa54-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaa54-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaa54-131">Response</span></span>
<span data-ttu-id="eaa54-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eaa54-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa54-133">Пример</span><span class="sxs-lookup"><span data-stu-id="eaa54-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaa54-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaa54-134">Request</span></span>
<span data-ttu-id="eaa54-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaa54-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

### <a name="response"></a><span data-ttu-id="eaa54-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaa54-136">Response</span></span>
<span data-ttu-id="eaa54-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaa54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
    "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
    "baseId": "Base Id value",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "displayVersion": "Display Version value",
    "lifecycleState": "draft",
    "platforms": "macOS",
    "technologies": "mdm",
    "templateFamily": "endpointSecurityAntivirus",
    "allowUnmanagedSettings": true,
    "settingTemplateCount": 4
  }
}
```




