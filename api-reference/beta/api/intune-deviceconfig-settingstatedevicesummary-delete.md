---
title: Удаление объекта settingStateDeviceSummary
description: Удаляет объект settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76fdb4b9d649056541c8def0e46ad46d46b478ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077235"
---
# <a name="delete-settingstatedevicesummary"></a><span data-ttu-id="791ea-103">Удаление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="791ea-103">Delete settingStateDeviceSummary</span></span>

<span data-ttu-id="791ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="791ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="791ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="791ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="791ea-107">Удаляет объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="791ea-107">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="791ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="791ea-108">Prerequisites</span></span>
<span data-ttu-id="791ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791ea-111">Permission type</span></span>|<span data-ttu-id="791ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="791ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="791ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="791ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="791ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="791ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791ea-116">Not supported.</span></span>|
|<span data-ttu-id="791ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791ea-117">Application</span></span>|<span data-ttu-id="791ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="791ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="791ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="791ea-120">Request headers</span></span>
|<span data-ttu-id="791ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="791ea-121">Header</span></span>|<span data-ttu-id="791ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="791ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="791ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="791ea-123">Authorization</span></span>|<span data-ttu-id="791ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="791ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="791ea-125">Accept</span></span>|<span data-ttu-id="791ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="791ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="791ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="791ea-127">Request body</span></span>
<span data-ttu-id="791ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="791ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="791ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="791ea-129">Response</span></span>
<span data-ttu-id="791ea-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="791ea-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="791ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="791ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="791ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="791ea-132">Request</span></span>
<span data-ttu-id="791ea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="791ea-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="791ea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="791ea-134">Response</span></span>
<span data-ttu-id="791ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="791ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






