---
title: Delete deviceConfigurationUserStatus
description: Удаляет объект deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28ecf5f3817177d42516988b3cbf57041b63dcdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011482"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="9403c-103">Delete deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="9403c-103">Delete deviceConfigurationUserStatus</span></span>

<span data-ttu-id="9403c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9403c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9403c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9403c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9403c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9403c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9403c-107">Удаляет объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9403c-107">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9403c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9403c-108">Prerequisites</span></span>
<span data-ttu-id="9403c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9403c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9403c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9403c-111">Permission type</span></span>|<span data-ttu-id="9403c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9403c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9403c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9403c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9403c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9403c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9403c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9403c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9403c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9403c-116">Not supported.</span></span>|
|<span data-ttu-id="9403c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9403c-117">Application</span></span>|<span data-ttu-id="9403c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9403c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9403c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9403c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="9403c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9403c-120">Request headers</span></span>
|<span data-ttu-id="9403c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9403c-121">Header</span></span>|<span data-ttu-id="9403c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9403c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9403c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9403c-123">Authorization</span></span>|<span data-ttu-id="9403c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9403c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9403c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9403c-125">Accept</span></span>|<span data-ttu-id="9403c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9403c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9403c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9403c-127">Request body</span></span>
<span data-ttu-id="9403c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9403c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9403c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9403c-129">Response</span></span>
<span data-ttu-id="9403c-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9403c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9403c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9403c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9403c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9403c-132">Request</span></span>
<span data-ttu-id="9403c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9403c-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="9403c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9403c-134">Response</span></span>
<span data-ttu-id="9403c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9403c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






