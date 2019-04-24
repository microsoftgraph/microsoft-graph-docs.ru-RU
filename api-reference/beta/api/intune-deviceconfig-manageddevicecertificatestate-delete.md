---
title: Удаление Манажеддевицецертификатестате
description: Удаляет объект Манажеддевицецертификатестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6f35280bc6ca5c6b213a2d3087cdafbc9827bcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518298"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="3aaaf-103">Удаление Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="3aaaf-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="3aaaf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3aaaf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aaaf-106">Удаляет объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="3aaaf-106">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3aaaf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3aaaf-107">Prerequisites</span></span>
<span data-ttu-id="3aaaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aaaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aaaf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3aaaf-110">Permission type</span></span>|<span data-ttu-id="3aaaf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3aaaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aaaf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3aaaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3aaaf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aaaf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3aaaf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3aaaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aaaf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-115">Not supported.</span></span>|
|<span data-ttu-id="3aaaf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3aaaf-116">Application</span></span>|<span data-ttu-id="3aaaf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aaaf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3aaaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3aaaf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3aaaf-119">Request headers</span></span>
|<span data-ttu-id="3aaaf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3aaaf-120">Header</span></span>|<span data-ttu-id="3aaaf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3aaaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aaaf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3aaaf-122">Authorization</span></span>|<span data-ttu-id="3aaaf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aaaf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3aaaf-124">Accept</span></span>|<span data-ttu-id="3aaaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3aaaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aaaf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3aaaf-126">Request body</span></span>
<span data-ttu-id="3aaaf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aaaf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aaaf-128">Response</span></span>
<span data-ttu-id="3aaaf-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3aaaf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3aaaf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3aaaf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3aaaf-131">Request</span></span>
<span data-ttu-id="3aaaf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="3aaaf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aaaf-133">Response</span></span>
<span data-ttu-id="3aaaf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3aaaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





