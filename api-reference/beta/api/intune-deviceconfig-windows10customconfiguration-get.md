---
title: Get windows10CustomConfiguration
description: Чтение свойств и связей объекта windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d45a31b3fe03eaa1c3e9cf31f2b8f99e7fc4675d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866491"
---
# <a name="get-windows10customconfiguration"></a><span data-ttu-id="72a63-103">Get windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="72a63-103">Get windows10CustomConfiguration</span></span>

<span data-ttu-id="72a63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72a63-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72a63-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72a63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72a63-107">Чтение свойств и связей объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72a63-107">Read properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72a63-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="72a63-108">Prerequisites</span></span>
<span data-ttu-id="72a63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72a63-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72a63-111">Permission type</span></span>|<span data-ttu-id="72a63-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72a63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72a63-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72a63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72a63-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72a63-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72a63-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72a63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72a63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a63-116">Not supported.</span></span>|
|<span data-ttu-id="72a63-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="72a63-117">Application</span></span>|<span data-ttu-id="72a63-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72a63-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72a63-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72a63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72a63-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72a63-120">Optional query parameters</span></span>
<span data-ttu-id="72a63-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72a63-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72a63-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72a63-122">Request headers</span></span>
|<span data-ttu-id="72a63-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72a63-123">Header</span></span>|<span data-ttu-id="72a63-124">Значение</span><span class="sxs-lookup"><span data-stu-id="72a63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72a63-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72a63-125">Authorization</span></span>|<span data-ttu-id="72a63-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72a63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72a63-127">Accept</span><span class="sxs-lookup"><span data-stu-id="72a63-127">Accept</span></span>|<span data-ttu-id="72a63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72a63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72a63-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72a63-129">Request body</span></span>
<span data-ttu-id="72a63-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72a63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72a63-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a63-131">Response</span></span>
<span data-ttu-id="72a63-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72a63-132">If successful, this method returns a `200 OK` response code and [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72a63-133">Пример</span><span class="sxs-lookup"><span data-stu-id="72a63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="72a63-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="72a63-134">Request</span></span>
<span data-ttu-id="72a63-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72a63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="72a63-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a63-136">Response</span></span>
<span data-ttu-id="72a63-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72a63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
    "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSetting",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "secretReferenceValueId": "Secret Reference Value Id value",
        "isEncrypted": true
      }
    ]
  }
}
```




