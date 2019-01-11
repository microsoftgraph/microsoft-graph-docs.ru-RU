---
title: Получение windowsIdentityProtectionConfiguration
description: Чтение свойства и связи объекта windowsIdentityProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fde8d4dcb8c7a5b94069466757d6c2ffb1351355
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880999"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="63591-103">Получение windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="63591-103">Get windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="63591-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63591-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63591-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63591-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63591-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63591-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63591-107">Чтение свойства и связи объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63591-107">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63591-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63591-108">Prerequisites</span></span>
<span data-ttu-id="63591-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63591-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63591-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63591-111">Permission type</span></span>|<span data-ttu-id="63591-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63591-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63591-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63591-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63591-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63591-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63591-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63591-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63591-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63591-116">Not supported.</span></span>|
|<span data-ttu-id="63591-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63591-117">Application</span></span>|<span data-ttu-id="63591-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63591-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63591-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63591-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63591-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63591-120">Optional query parameters</span></span>
<span data-ttu-id="63591-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="63591-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="63591-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63591-122">Request headers</span></span>
|<span data-ttu-id="63591-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63591-123">Header</span></span>|<span data-ttu-id="63591-124">Значение</span><span class="sxs-lookup"><span data-stu-id="63591-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63591-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63591-125">Authorization</span></span>|<span data-ttu-id="63591-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="63591-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63591-127">Accept</span><span class="sxs-lookup"><span data-stu-id="63591-127">Accept</span></span>|<span data-ttu-id="63591-128">application/json</span><span class="sxs-lookup"><span data-stu-id="63591-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63591-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63591-129">Request body</span></span>
<span data-ttu-id="63591-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63591-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63591-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="63591-131">Response</span></span>
<span data-ttu-id="63591-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="63591-132">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63591-133">Пример</span><span class="sxs-lookup"><span data-stu-id="63591-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="63591-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="63591-134">Request</span></span>
<span data-ttu-id="63591-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63591-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="63591-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="63591-136">Response</span></span>
<span data-ttu-id="63591-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63591-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

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





