---
title: Get deviceConfigurationAssignment
description: Чтение свойств и связей объекта deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61d206b2f9158261333ddd2dd58cf140340085c0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927442"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="37612-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="37612-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="37612-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37612-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37612-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37612-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37612-106">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37612-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37612-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="37612-107">Prerequisites</span></span>
<span data-ttu-id="37612-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37612-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37612-110">Permission type</span></span>|<span data-ttu-id="37612-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37612-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37612-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37612-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37612-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37612-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37612-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37612-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37612-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37612-115">Not supported.</span></span>|
|<span data-ttu-id="37612-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37612-116">Application</span></span>|<span data-ttu-id="37612-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37612-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37612-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37612-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37612-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37612-119">Optional query parameters</span></span>
<span data-ttu-id="37612-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37612-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37612-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37612-121">Request headers</span></span>
|<span data-ttu-id="37612-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37612-122">Header</span></span>|<span data-ttu-id="37612-123">Значение</span><span class="sxs-lookup"><span data-stu-id="37612-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37612-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37612-124">Authorization</span></span>|<span data-ttu-id="37612-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37612-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37612-126">Accept</span><span class="sxs-lookup"><span data-stu-id="37612-126">Accept</span></span>|<span data-ttu-id="37612-127">application/json</span><span class="sxs-lookup"><span data-stu-id="37612-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37612-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37612-128">Request body</span></span>
<span data-ttu-id="37612-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37612-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37612-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="37612-130">Response</span></span>
<span data-ttu-id="37612-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37612-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37612-132">Пример</span><span class="sxs-lookup"><span data-stu-id="37612-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="37612-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="37612-133">Request</span></span>
<span data-ttu-id="37612-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37612-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="37612-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="37612-135">Response</span></span>
<span data-ttu-id="37612-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37612-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




