---
title: Удаление объекта settingStateDeviceSummary
description: Удаляет объект settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 666e5115e05367c6df572e7d42f6233c2b4e9a04
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083034"
---
# <a name="delete-settingstatedevicesummary"></a><span data-ttu-id="062bc-103">Удаление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="062bc-103">Delete settingStateDeviceSummary</span></span>

> <span data-ttu-id="062bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="062bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="062bc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="062bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="062bc-106">Удаляет объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="062bc-106">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="062bc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="062bc-107">Prerequisites</span></span>
<span data-ttu-id="062bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="062bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="062bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="062bc-110">Permission type</span></span>|<span data-ttu-id="062bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="062bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="062bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="062bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="062bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="062bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="062bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="062bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="062bc-115">Not supported.</span></span>|
|<span data-ttu-id="062bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="062bc-116">Application</span></span>|<span data-ttu-id="062bc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062bc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="062bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="062bc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="062bc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="062bc-119">Request headers</span></span>
|<span data-ttu-id="062bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="062bc-120">Header</span></span>|<span data-ttu-id="062bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="062bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="062bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="062bc-122">Authorization</span></span>|<span data-ttu-id="062bc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="062bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="062bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="062bc-124">Accept</span></span>|<span data-ttu-id="062bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="062bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="062bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="062bc-126">Request body</span></span>
<span data-ttu-id="062bc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="062bc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="062bc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="062bc-128">Response</span></span>
<span data-ttu-id="062bc-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="062bc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="062bc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="062bc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="062bc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="062bc-131">Request</span></span>
<span data-ttu-id="062bc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="062bc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="062bc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="062bc-133">Response</span></span>
<span data-ttu-id="062bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="062bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






