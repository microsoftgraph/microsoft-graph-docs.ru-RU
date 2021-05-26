---
title: Список deviceManagementConfigurationPolicyTemplates
description: Список свойств и связей объектов deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abc6d85ecf76c4235d0277ceaf50f3f0655e4822
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665885"
---
# <a name="list-devicemanagementconfigurationpolicytemplates"></a><span data-ttu-id="2ce38-103">Список deviceManagementConfigurationPolicyTemplates</span><span class="sxs-lookup"><span data-stu-id="2ce38-103">List deviceManagementConfigurationPolicyTemplates</span></span>

<span data-ttu-id="2ce38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ce38-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ce38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ce38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ce38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ce38-107">Список свойств и связей [объектов deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)</span><span class="sxs-lookup"><span data-stu-id="2ce38-107">List properties and relationships of the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ce38-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ce38-108">Prerequisites</span></span>
<span data-ttu-id="2ce38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ce38-111">Permission type</span></span>|<span data-ttu-id="2ce38-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ce38-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ce38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ce38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ce38-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce38-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ce38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ce38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ce38-116">Not supported.</span></span>|
|<span data-ttu-id="2ce38-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ce38-117">Application</span></span>|<span data-ttu-id="2ce38-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce38-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ce38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a><span data-ttu-id="2ce38-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ce38-120">Request headers</span></span>
|<span data-ttu-id="2ce38-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ce38-121">Header</span></span>|<span data-ttu-id="2ce38-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ce38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ce38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce38-123">Authorization</span></span>|<span data-ttu-id="2ce38-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ce38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ce38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ce38-125">Accept</span></span>|<span data-ttu-id="2ce38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ce38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce38-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ce38-127">Request body</span></span>
<span data-ttu-id="2ce38-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ce38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce38-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ce38-129">Response</span></span>
<span data-ttu-id="2ce38-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce38-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ce38-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ce38-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ce38-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ce38-132">Request</span></span>
<span data-ttu-id="2ce38-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce38-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
```

### <a name="response"></a><span data-ttu-id="2ce38-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ce38-134">Response</span></span>
<span data-ttu-id="2ce38-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ce38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 587

{
  "value": [
    {
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
  ]
}
```




