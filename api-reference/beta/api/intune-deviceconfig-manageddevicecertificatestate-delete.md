---
title: Удаление managedDeviceCertificateState
description: Удаляет managedDeviceCertificateState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: da38b1feaeae9911d887dfdda8ca5845be0dae80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982535"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="a73de-103">Удаление managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="a73de-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="a73de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a73de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a73de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a73de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a73de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a73de-107">Удаляет [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="a73de-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a73de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a73de-108">Prerequisites</span></span>
<span data-ttu-id="a73de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a73de-111">Permission type</span></span>|<span data-ttu-id="a73de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a73de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a73de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a73de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a73de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a73de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a73de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a73de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73de-116">Not supported.</span></span>|
|<span data-ttu-id="a73de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a73de-117">Application</span></span>|<span data-ttu-id="a73de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a73de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a73de-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a73de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a73de-120">Request headers</span></span>
|<span data-ttu-id="a73de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a73de-121">Header</span></span>|<span data-ttu-id="a73de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a73de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a73de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a73de-123">Authorization</span></span>|<span data-ttu-id="a73de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a73de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a73de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a73de-125">Accept</span></span>|<span data-ttu-id="a73de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a73de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a73de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a73de-127">Request body</span></span>
<span data-ttu-id="a73de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a73de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a73de-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a73de-129">Response</span></span>
<span data-ttu-id="a73de-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a73de-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a73de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a73de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a73de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a73de-132">Request</span></span>
<span data-ttu-id="a73de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a73de-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="a73de-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a73de-134">Response</span></span>
<span data-ttu-id="a73de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a73de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





