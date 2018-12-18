---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 020390ddc45159daf1717cd6cb3cc96fce40f882
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327393"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="8e937-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8e937-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="8e937-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e937-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e937-105">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e937-105">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e937-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8e937-106">Prerequisites</span></span>
<span data-ttu-id="8e937-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e937-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e937-109">Permission type</span></span>|<span data-ttu-id="8e937-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e937-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e937-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e937-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e937-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e937-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8e937-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e937-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e937-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e937-114">Not supported.</span></span>|
|<span data-ttu-id="8e937-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e937-115">Application</span></span>|<span data-ttu-id="8e937-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e937-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e937-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e937-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e937-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e937-118">Optional query parameters</span></span>
<span data-ttu-id="8e937-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e937-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e937-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e937-120">Request headers</span></span>
|<span data-ttu-id="8e937-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e937-121">Header</span></span>|<span data-ttu-id="8e937-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e937-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e937-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e937-123">Authorization</span></span>|<span data-ttu-id="8e937-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e937-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e937-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e937-125">Accept</span></span>|<span data-ttu-id="8e937-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e937-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e937-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e937-127">Request body</span></span>
<span data-ttu-id="8e937-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e937-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e937-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e937-129">Response</span></span>
<span data-ttu-id="8e937-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8e937-130">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e937-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8e937-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e937-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e937-132">Request</span></span>
<span data-ttu-id="8e937-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e937-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="8e937-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e937-134">Response</span></span>
<span data-ttu-id="8e937-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8e937-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1197

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true
  }
}
```



