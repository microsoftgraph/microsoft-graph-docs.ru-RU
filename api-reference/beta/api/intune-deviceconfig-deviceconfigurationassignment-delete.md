---
title: Delete deviceConfigurationAssignment
description: Удаляет объект deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9011c5bcf670edb7f45c7cc06b633dab79758444
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346046"
---
# <a name="delete-deviceconfigurationassignment"></a><span data-ttu-id="7a15a-103">Delete deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7a15a-103">Delete deviceConfigurationAssignment</span></span>

> <span data-ttu-id="7a15a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a15a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a15a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a15a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a15a-106">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7a15a-106">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a15a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7a15a-107">Prerequisites</span></span>
<span data-ttu-id="7a15a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a15a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a15a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a15a-110">Permission type</span></span>|<span data-ttu-id="7a15a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a15a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a15a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a15a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a15a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a15a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a15a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a15a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a15a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a15a-115">Not supported.</span></span>|
|<span data-ttu-id="7a15a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a15a-116">Application</span></span>|<span data-ttu-id="7a15a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a15a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a15a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a15a-118">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7a15a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a15a-119">Request headers</span></span>
|<span data-ttu-id="7a15a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a15a-120">Header</span></span>|<span data-ttu-id="7a15a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7a15a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a15a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a15a-122">Authorization</span></span>|<span data-ttu-id="7a15a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a15a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a15a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7a15a-124">Accept</span></span>|<span data-ttu-id="7a15a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a15a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a15a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a15a-126">Request body</span></span>
<span data-ttu-id="7a15a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a15a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a15a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a15a-128">Response</span></span>
<span data-ttu-id="7a15a-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a15a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a15a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7a15a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a15a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a15a-131">Request</span></span>
<span data-ttu-id="7a15a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a15a-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7a15a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a15a-133">Response</span></span>
<span data-ttu-id="7a15a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a15a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






