---
title: Get macOSCompliancePolicy
description: Чтение свойств и связей объекта macOSCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 26e06cb7b633aacc149b4790be99d0fa74b12c67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353566"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="a0e63-103">Get macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a0e63-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="a0e63-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0e63-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0e63-105">Чтение свойств и связей объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0e63-105">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0e63-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e63-106">Prerequisites</span></span>
<span data-ttu-id="a0e63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e63-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e63-109">Permission type</span></span>|<span data-ttu-id="a0e63-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0e63-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e63-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0e63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e63-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0e63-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0e63-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0e63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e63-114">Not supported.</span></span>|
|<span data-ttu-id="a0e63-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0e63-115">Application</span></span>|<span data-ttu-id="a0e63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e63-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0e63-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0e63-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0e63-118">Optional query parameters</span></span>
<span data-ttu-id="a0e63-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0e63-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0e63-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0e63-120">Request headers</span></span>
|<span data-ttu-id="a0e63-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0e63-121">Header</span></span>|<span data-ttu-id="a0e63-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a0e63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e63-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0e63-123">Authorization</span></span>|<span data-ttu-id="a0e63-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a0e63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0e63-125">Accept</span></span>|<span data-ttu-id="a0e63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e63-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0e63-127">Request body</span></span>
<span data-ttu-id="a0e63-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0e63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0e63-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0e63-129">Response</span></span>
<span data-ttu-id="a0e63-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0e63-130">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e63-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a0e63-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0e63-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0e63-132">Request</span></span>
<span data-ttu-id="a0e63-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0e63-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a0e63-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0e63-134">Response</span></span>
<span data-ttu-id="a0e63-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a0e63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```



