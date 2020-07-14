---
title: Удаление Манажеддевицецертификатестате
description: Удаляет объект Манажеддевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c66af6b517cd68ff475ab04fbc6bf244b7988a53
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122891"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="87a12-103">Удаление Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="87a12-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="87a12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87a12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87a12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87a12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a12-107">Удаляет объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="87a12-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87a12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87a12-108">Prerequisites</span></span>
<span data-ttu-id="87a12-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="87a12-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="87a12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87a12-111">Permission type</span></span>|<span data-ttu-id="87a12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87a12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87a12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87a12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87a12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87a12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a12-116">Not supported.</span></span>|
|<span data-ttu-id="87a12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87a12-117">Application</span></span>|<span data-ttu-id="87a12-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a12-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87a12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="87a12-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87a12-120">Request headers</span></span>
|<span data-ttu-id="87a12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87a12-121">Header</span></span>|<span data-ttu-id="87a12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87a12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a12-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87a12-123">Authorization</span></span>|<span data-ttu-id="87a12-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87a12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87a12-125">Accept</span></span>|<span data-ttu-id="87a12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87a12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87a12-127">Request body</span></span>
<span data-ttu-id="87a12-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87a12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87a12-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87a12-129">Response</span></span>
<span data-ttu-id="87a12-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="87a12-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="87a12-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87a12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87a12-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87a12-132">Request</span></span>
<span data-ttu-id="87a12-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87a12-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="87a12-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87a12-134">Response</span></span>
<span data-ttu-id="87a12-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="87a12-135">Here is an example of the response.</span></span> <span data-ttu-id="87a12-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="87a12-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87a12-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="87a12-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



