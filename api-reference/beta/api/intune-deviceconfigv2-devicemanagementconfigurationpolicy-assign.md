---
title: Политика конфигурации управления устройствами назначает действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c92091d06a7ad872e4e8853bd85521be61a4adb9
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666136"
---
# <a name="device-management-configuration-policy-assign-action"></a><span data-ttu-id="40936-103">Политика конфигурации управления устройствами назначает действие</span><span class="sxs-lookup"><span data-stu-id="40936-103">Device management configuration policy assign action</span></span>

<span data-ttu-id="40936-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40936-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40936-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40936-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40936-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40936-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40936-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="40936-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40936-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40936-108">Prerequisites</span></span>
<span data-ttu-id="40936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40936-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40936-111">Permission type</span></span>|<span data-ttu-id="40936-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40936-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40936-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40936-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40936-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40936-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40936-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40936-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40936-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40936-116">Not supported.</span></span>|
|<span data-ttu-id="40936-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="40936-117">Application</span></span>|<span data-ttu-id="40936-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40936-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40936-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40936-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="40936-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40936-120">Request headers</span></span>
|<span data-ttu-id="40936-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40936-121">Header</span></span>|<span data-ttu-id="40936-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40936-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40936-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40936-123">Authorization</span></span>|<span data-ttu-id="40936-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40936-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40936-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40936-125">Accept</span></span>|<span data-ttu-id="40936-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40936-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40936-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40936-127">Request body</span></span>
<span data-ttu-id="40936-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40936-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="40936-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="40936-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="40936-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40936-130">Property</span></span>|<span data-ttu-id="40936-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40936-131">Type</span></span>|<span data-ttu-id="40936-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40936-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40936-133">assignments</span><span class="sxs-lookup"><span data-stu-id="40936-133">assignments</span></span>|<span data-ttu-id="40936-134">[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="40936-134">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="40936-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="40936-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40936-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="40936-136">Response</span></span>
<span data-ttu-id="40936-137">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [коллекцию deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="40936-137">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40936-138">Пример</span><span class="sxs-lookup"><span data-stu-id="40936-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="40936-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="40936-139">Request</span></span>
<span data-ttu-id="40936-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40936-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign

Content-type: application/json
Content-length: 524

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="40936-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="40936-141">Response</span></span>
<span data-ttu-id="40936-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40936-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




