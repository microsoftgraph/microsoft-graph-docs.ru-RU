---
title: Delete deviceConfigurationAssignment
description: Удаляет объект deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adae73cb2b48026b5cc0531020d092fcef0ed657
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011538"
---
# <a name="delete-deviceconfigurationassignment"></a><span data-ttu-id="eb57e-103">Delete deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eb57e-103">Delete deviceConfigurationAssignment</span></span>

<span data-ttu-id="eb57e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb57e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb57e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb57e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb57e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb57e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb57e-107">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eb57e-107">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb57e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="eb57e-108">Prerequisites</span></span>
<span data-ttu-id="eb57e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb57e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb57e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb57e-111">Permission type</span></span>|<span data-ttu-id="eb57e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb57e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb57e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb57e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb57e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb57e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb57e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb57e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb57e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb57e-116">Not supported.</span></span>|
|<span data-ttu-id="eb57e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="eb57e-117">Application</span></span>|<span data-ttu-id="eb57e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb57e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb57e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb57e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eb57e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eb57e-120">Request headers</span></span>
|<span data-ttu-id="eb57e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb57e-121">Header</span></span>|<span data-ttu-id="eb57e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eb57e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb57e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb57e-123">Authorization</span></span>|<span data-ttu-id="eb57e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb57e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb57e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb57e-125">Accept</span></span>|<span data-ttu-id="eb57e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb57e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb57e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb57e-127">Request body</span></span>
<span data-ttu-id="eb57e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb57e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb57e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb57e-129">Response</span></span>
<span data-ttu-id="eb57e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb57e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eb57e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="eb57e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb57e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb57e-132">Request</span></span>
<span data-ttu-id="eb57e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb57e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="eb57e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb57e-134">Response</span></span>
<span data-ttu-id="eb57e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb57e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






