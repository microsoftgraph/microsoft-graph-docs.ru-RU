---
title: Получение Андроидворкпрофилинтерприсевификонфигуратион
description: Чтение свойств и связей объекта Андроидворкпрофилинтерприсевификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfde5ef2e9ce0127a7af3db8007ced732df5ec81
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963746"
---
# <a name="get-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="815ce-103">Получение Андроидворкпрофилинтерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="815ce-103">Get androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="815ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="815ce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="815ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="815ce-106">Чтение свойств и связей объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="815ce-106">Read properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="815ce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="815ce-107">Prerequisites</span></span>
<span data-ttu-id="815ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="815ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="815ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="815ce-110">Permission type</span></span>|<span data-ttu-id="815ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="815ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="815ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="815ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="815ce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="815ce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="815ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="815ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="815ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815ce-115">Not supported.</span></span>|
|<span data-ttu-id="815ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="815ce-116">Application</span></span>|<span data-ttu-id="815ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="815ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="815ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="815ce-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="815ce-119">Optional query parameters</span></span>
<span data-ttu-id="815ce-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="815ce-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="815ce-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="815ce-121">Request headers</span></span>
|<span data-ttu-id="815ce-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="815ce-122">Header</span></span>|<span data-ttu-id="815ce-123">Значение</span><span class="sxs-lookup"><span data-stu-id="815ce-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="815ce-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="815ce-124">Authorization</span></span>|<span data-ttu-id="815ce-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="815ce-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="815ce-126">Accept</span><span class="sxs-lookup"><span data-stu-id="815ce-126">Accept</span></span>|<span data-ttu-id="815ce-127">application/json</span><span class="sxs-lookup"><span data-stu-id="815ce-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="815ce-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="815ce-128">Request body</span></span>
<span data-ttu-id="815ce-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="815ce-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="815ce-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="815ce-130">Response</span></span>
<span data-ttu-id="815ce-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="815ce-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="815ce-132">Пример</span><span class="sxs-lookup"><span data-stu-id="815ce-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="815ce-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="815ce-133">Request</span></span>
<span data-ttu-id="815ce-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="815ce-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="815ce-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="815ce-135">Response</span></span>
<span data-ttu-id="815ce-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="815ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1009

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
    "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaEnterprise",
    "eapType": "eapTtls",
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
    "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```




