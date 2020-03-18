---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4defc4f2639ad319d8bbc4ed4e2590f5e4a8d67f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42754540"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="51376-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="51376-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="51376-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51376-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51376-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51376-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51376-106">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51376-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51376-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51376-107">Prerequisites</span></span>
<span data-ttu-id="51376-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51376-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51376-110">Permission type</span></span>|<span data-ttu-id="51376-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51376-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51376-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51376-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51376-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51376-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51376-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51376-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51376-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51376-115">Not supported.</span></span>|
|<span data-ttu-id="51376-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51376-116">Application</span></span>|<span data-ttu-id="51376-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51376-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51376-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51376-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="51376-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51376-119">Request headers</span></span>
|<span data-ttu-id="51376-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51376-120">Header</span></span>|<span data-ttu-id="51376-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51376-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51376-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51376-122">Authorization</span></span>|<span data-ttu-id="51376-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51376-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51376-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51376-124">Accept</span></span>|<span data-ttu-id="51376-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51376-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51376-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51376-126">Request body</span></span>
<span data-ttu-id="51376-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51376-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51376-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="51376-128">Response</span></span>
<span data-ttu-id="51376-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51376-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51376-130">Пример</span><span class="sxs-lookup"><span data-stu-id="51376-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="51376-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="51376-131">Request</span></span>
<span data-ttu-id="51376-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51376-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="51376-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="51376-133">Response</span></span>
<span data-ttu-id="51376-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51376-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




