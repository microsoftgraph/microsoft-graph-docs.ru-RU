---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bdc157b5e626463b21c8ebc9a8ea91fe9fcc365
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346053"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="331c4-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="331c4-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="331c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="331c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="331c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="331c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="331c4-106">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="331c4-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="331c4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="331c4-107">Prerequisites</span></span>
<span data-ttu-id="331c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="331c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="331c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="331c4-110">Permission type</span></span>|<span data-ttu-id="331c4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="331c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="331c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="331c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="331c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="331c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="331c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="331c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="331c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="331c4-115">Not supported.</span></span>|
|<span data-ttu-id="331c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="331c4-116">Application</span></span>|<span data-ttu-id="331c4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="331c4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="331c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="331c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="331c4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="331c4-119">Request headers</span></span>
|<span data-ttu-id="331c4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="331c4-120">Header</span></span>|<span data-ttu-id="331c4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="331c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="331c4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="331c4-122">Authorization</span></span>|<span data-ttu-id="331c4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="331c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="331c4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="331c4-124">Accept</span></span>|<span data-ttu-id="331c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="331c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="331c4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="331c4-126">Request body</span></span>
<span data-ttu-id="331c4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="331c4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="331c4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="331c4-128">Response</span></span>
<span data-ttu-id="331c4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="331c4-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="331c4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="331c4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="331c4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="331c4-131">Request</span></span>
<span data-ttu-id="331c4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="331c4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="331c4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="331c4-133">Response</span></span>
<span data-ttu-id="331c4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="331c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






