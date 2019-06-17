---
title: Список Девицеконфигуратионграупассигнментс
description: Список свойств и связей объектов deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f17d617091a363ea5e8f07eabd38b194431a6d9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967680"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="ab533-103">Список Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="ab533-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="ab533-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab533-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab533-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab533-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab533-106">Список свойств и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ab533-106">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab533-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab533-107">Prerequisites</span></span>
<span data-ttu-id="ab533-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab533-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab533-110">Permission type</span></span>|<span data-ttu-id="ab533-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab533-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab533-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab533-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab533-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab533-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab533-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab533-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab533-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab533-115">Not supported.</span></span>|
|<span data-ttu-id="ab533-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab533-116">Application</span></span>|<span data-ttu-id="ab533-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab533-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab533-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab533-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ab533-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab533-119">Request headers</span></span>
|<span data-ttu-id="ab533-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab533-120">Header</span></span>|<span data-ttu-id="ab533-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab533-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab533-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab533-122">Authorization</span></span>|<span data-ttu-id="ab533-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab533-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab533-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ab533-124">Accept</span></span>|<span data-ttu-id="ab533-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab533-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab533-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab533-126">Request body</span></span>
<span data-ttu-id="ab533-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab533-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab533-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab533-128">Response</span></span>
<span data-ttu-id="ab533-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab533-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab533-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ab533-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab533-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab533-131">Request</span></span>
<span data-ttu-id="ab533-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab533-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="ab533-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab533-133">Response</span></span>
<span data-ttu-id="ab533-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab533-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```





