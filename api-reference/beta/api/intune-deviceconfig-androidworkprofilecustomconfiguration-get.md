---
title: Get AndroidWorkProfileCustomConfiguration
description: Чтение свойств и связей объекта AndroidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14a49df003a3c8a9d80eda32a7f37f063a3bd6b6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864545"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="bfd0b-103">Get AndroidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfd0b-103">Get androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="bfd0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfd0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfd0b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfd0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfd0b-107">Чтение свойств и связей [объекта AndroidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bfd0b-107">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfd0b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bfd0b-108">Prerequisites</span></span>
<span data-ttu-id="bfd0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfd0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfd0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfd0b-111">Permission type</span></span>|<span data-ttu-id="bfd0b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfd0b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfd0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfd0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfd0b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd0b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfd0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfd0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfd0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-116">Not supported.</span></span>|
|<span data-ttu-id="bfd0b-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="bfd0b-117">Application</span></span>|<span data-ttu-id="bfd0b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd0b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfd0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfd0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfd0b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfd0b-120">Optional query parameters</span></span>
<span data-ttu-id="bfd0b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfd0b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfd0b-122">Request headers</span></span>
|<span data-ttu-id="bfd0b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfd0b-123">Header</span></span>|<span data-ttu-id="bfd0b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bfd0b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfd0b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfd0b-125">Authorization</span></span>|<span data-ttu-id="bfd0b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfd0b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bfd0b-127">Accept</span></span>|<span data-ttu-id="bfd0b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bfd0b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfd0b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfd0b-129">Request body</span></span>
<span data-ttu-id="bfd0b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfd0b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfd0b-131">Response</span></span>
<span data-ttu-id="bfd0b-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfd0b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bfd0b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfd0b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfd0b-134">Request</span></span>
<span data-ttu-id="bfd0b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bfd0b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfd0b-136">Response</span></span>
<span data-ttu-id="bfd0b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfd0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1623

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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




