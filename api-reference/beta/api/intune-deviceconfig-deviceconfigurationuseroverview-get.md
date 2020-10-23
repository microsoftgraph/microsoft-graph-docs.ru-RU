---
title: Get deviceConfigurationUserOverview
description: Чтение свойств и связей объекта deviceConfigurationUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36f827dbe5773326335e42b8c855687128484b3e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725726"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="f2522-103">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f2522-103">Get deviceConfigurationUserOverview</span></span>

<span data-ttu-id="f2522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2522-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2522-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2522-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2522-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2522-107">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f2522-107">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2522-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f2522-108">Prerequisites</span></span>
<span data-ttu-id="f2522-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2522-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2522-111">Permission type</span></span>|<span data-ttu-id="f2522-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2522-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2522-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2522-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2522-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2522-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2522-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2522-116">Not supported.</span></span>|
|<span data-ttu-id="f2522-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2522-117">Application</span></span>|<span data-ttu-id="f2522-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2522-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2522-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2522-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2522-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2522-120">Optional query parameters</span></span>
<span data-ttu-id="f2522-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2522-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2522-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2522-122">Request headers</span></span>
|<span data-ttu-id="f2522-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2522-123">Header</span></span>|<span data-ttu-id="f2522-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f2522-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2522-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2522-125">Authorization</span></span>|<span data-ttu-id="f2522-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2522-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2522-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f2522-127">Accept</span></span>|<span data-ttu-id="f2522-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2522-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2522-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2522-129">Request body</span></span>
<span data-ttu-id="f2522-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2522-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2522-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2522-131">Response</span></span>
<span data-ttu-id="f2522-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2522-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2522-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f2522-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2522-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2522-134">Request</span></span>
<span data-ttu-id="f2522-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2522-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="f2522-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2522-136">Response</span></span>
<span data-ttu-id="f2522-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2522-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





