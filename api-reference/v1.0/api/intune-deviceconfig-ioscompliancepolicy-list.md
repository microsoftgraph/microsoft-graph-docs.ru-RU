---
title: Перечисление объектов iosCompliancePolicy
description: Список свойств и связей объектов iosCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2e93b42bfa0707f751285760e50255e6b9ab569
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368367"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="470e4-103">Перечисление объектов iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="470e4-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="470e4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="470e4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="470e4-105">Список свойств и связей объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="470e4-105">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="470e4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="470e4-106">Prerequisites</span></span>
<span data-ttu-id="470e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="470e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="470e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="470e4-109">Permission type</span></span>|<span data-ttu-id="470e4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="470e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="470e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="470e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="470e4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="470e4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="470e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="470e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="470e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="470e4-114">Not supported.</span></span>|
|<span data-ttu-id="470e4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="470e4-115">Application</span></span>|<span data-ttu-id="470e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="470e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="470e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="470e4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="470e4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="470e4-118">Request headers</span></span>
|<span data-ttu-id="470e4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="470e4-119">Header</span></span>|<span data-ttu-id="470e4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="470e4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="470e4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="470e4-121">Authorization</span></span>|<span data-ttu-id="470e4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="470e4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="470e4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="470e4-123">Accept</span></span>|<span data-ttu-id="470e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="470e4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="470e4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="470e4-125">Request body</span></span>
<span data-ttu-id="470e4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="470e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="470e4-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="470e4-127">Response</span></span>
<span data-ttu-id="470e4-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="470e4-128">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="470e4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="470e4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="470e4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="470e4-130">Request</span></span>
<span data-ttu-id="470e4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="470e4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="470e4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="470e4-132">Response</span></span>
<span data-ttu-id="470e4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="470e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
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
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```




