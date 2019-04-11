---
title: Получение Виндовсидентитипротектионконфигуратион
description: Чтение свойств и связей объекта Виндовсидентитипротектионконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fed21c47211e7d1774d18bc0edbfab3bc3f1ca39
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791805"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="50ddd-103">Получение Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="50ddd-103">Get windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="50ddd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50ddd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ddd-106">Чтение свойств и связей объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="50ddd-106">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50ddd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50ddd-107">Prerequisites</span></span>
<span data-ttu-id="50ddd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ddd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50ddd-110">Permission type</span></span>|<span data-ttu-id="50ddd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50ddd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50ddd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50ddd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50ddd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50ddd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50ddd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50ddd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50ddd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ddd-115">Not supported.</span></span>|
|<span data-ttu-id="50ddd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50ddd-116">Application</span></span>|<span data-ttu-id="50ddd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ddd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50ddd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50ddd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50ddd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50ddd-119">Optional query parameters</span></span>
<span data-ttu-id="50ddd-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50ddd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50ddd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50ddd-121">Request headers</span></span>
|<span data-ttu-id="50ddd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50ddd-122">Header</span></span>|<span data-ttu-id="50ddd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="50ddd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50ddd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50ddd-124">Authorization</span></span>|<span data-ttu-id="50ddd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50ddd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50ddd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="50ddd-126">Accept</span></span>|<span data-ttu-id="50ddd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50ddd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ddd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50ddd-128">Request body</span></span>
<span data-ttu-id="50ddd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50ddd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ddd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="50ddd-130">Response</span></span>
<span data-ttu-id="50ddd-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50ddd-131">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ddd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50ddd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ddd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="50ddd-133">Request</span></span>
<span data-ttu-id="50ddd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50ddd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50ddd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="50ddd-135">Response</span></span>
<span data-ttu-id="50ddd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50ddd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
    "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "useSecurityKeyForSignin": true,
    "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "pinExpirationInDays": 3,
    "pinPreviousBlockCount": 5,
    "pinRecoveryEnabled": true,
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "useCertificatesForOnPremisesAuthEnabled": true,
    "windowsHelloForBusinessBlocked": true
  }
}
```





