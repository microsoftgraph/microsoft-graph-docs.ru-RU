---
title: Delete deviceConfigurationUserStatus
description: Удаляет объект deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a7f4b899a94e0d94efc39de19a2a3a2a85fe6fd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164185"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="9ae44-103">Delete deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="9ae44-103">Delete deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="9ae44-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ae44-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ae44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ae44-106">Удаляет объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9ae44-106">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ae44-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae44-107">Prerequisites</span></span>
<span data-ttu-id="9ae44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ae44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ae44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae44-110">Permission type</span></span>|<span data-ttu-id="9ae44-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ae44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ae44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ae44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ae44-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ae44-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ae44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ae44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ae44-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae44-115">Not supported.</span></span>|
|<span data-ttu-id="9ae44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ae44-116">Application</span></span>|<span data-ttu-id="9ae44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ae44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ae44-118">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="9ae44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ae44-119">Request headers</span></span>
|<span data-ttu-id="9ae44-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ae44-120">Header</span></span>|<span data-ttu-id="9ae44-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ae44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ae44-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ae44-122">Authorization</span></span>|<span data-ttu-id="9ae44-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9ae44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ae44-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9ae44-124">Accept</span></span>|<span data-ttu-id="9ae44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ae44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ae44-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ae44-126">Request body</span></span>
<span data-ttu-id="9ae44-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ae44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ae44-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae44-128">Response</span></span>
<span data-ttu-id="9ae44-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ae44-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ae44-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9ae44-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ae44-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae44-131">Request</span></span>
<span data-ttu-id="9ae44-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae44-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="9ae44-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="9ae44-133">Response</span></span>
<span data-ttu-id="9ae44-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ae44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




