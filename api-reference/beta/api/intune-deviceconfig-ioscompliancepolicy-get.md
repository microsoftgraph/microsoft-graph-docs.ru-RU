---
title: Get iosCompliancePolicy
description: Чтение свойств и связей объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c8c5ed3263a85b9f1fa2ddf9c2b10e77fa8fa8f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877863"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="82130-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="82130-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="82130-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82130-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82130-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82130-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82130-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82130-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82130-107">Чтение свойств и связей объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82130-107">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82130-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="82130-108">Prerequisites</span></span>
<span data-ttu-id="82130-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82130-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82130-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82130-111">Permission type</span></span>|<span data-ttu-id="82130-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82130-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82130-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82130-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82130-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82130-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82130-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82130-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82130-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82130-116">Not supported.</span></span>|
|<span data-ttu-id="82130-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82130-117">Application</span></span>|<span data-ttu-id="82130-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82130-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82130-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82130-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82130-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82130-120">Optional query parameters</span></span>
<span data-ttu-id="82130-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82130-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82130-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82130-122">Request headers</span></span>
|<span data-ttu-id="82130-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82130-123">Header</span></span>|<span data-ttu-id="82130-124">Значение</span><span class="sxs-lookup"><span data-stu-id="82130-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82130-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="82130-125">Authorization</span></span>|<span data-ttu-id="82130-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82130-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82130-127">Accept</span><span class="sxs-lookup"><span data-stu-id="82130-127">Accept</span></span>|<span data-ttu-id="82130-128">application/json</span><span class="sxs-lookup"><span data-stu-id="82130-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82130-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82130-129">Request body</span></span>
<span data-ttu-id="82130-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82130-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82130-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="82130-131">Response</span></span>
<span data-ttu-id="82130-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82130-132">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82130-133">Пример</span><span class="sxs-lookup"><span data-stu-id="82130-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="82130-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="82130-134">Request</span></span>
<span data-ttu-id="82130-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82130-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="82130-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="82130-136">Response</span></span>
<span data-ttu-id="82130-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82130-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1376

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true,
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ]
  }
}
```





