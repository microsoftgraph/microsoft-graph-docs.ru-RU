---
title: Перечисление объектов macOSCompliancePolicy
description: Список свойств и связей объектов macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97883e78e1ac673002c906d804b27419ceaae567
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997535"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="af4b5-103">Перечисление объектов macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="af4b5-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="af4b5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af4b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af4b5-105">Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="af4b5-105">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af4b5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af4b5-106">Prerequisites</span></span>
<span data-ttu-id="af4b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af4b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af4b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af4b5-109">Permission type</span></span>|<span data-ttu-id="af4b5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af4b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af4b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af4b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af4b5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af4b5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af4b5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af4b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af4b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4b5-114">Not supported.</span></span>|
|<span data-ttu-id="af4b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af4b5-115">Application</span></span>|<span data-ttu-id="af4b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af4b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af4b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="af4b5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af4b5-118">Request headers</span></span>
|<span data-ttu-id="af4b5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af4b5-119">Header</span></span>|<span data-ttu-id="af4b5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="af4b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af4b5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af4b5-121">Authorization</span></span>|<span data-ttu-id="af4b5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af4b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af4b5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="af4b5-123">Accept</span></span>|<span data-ttu-id="af4b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af4b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af4b5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af4b5-125">Request body</span></span>
<span data-ttu-id="af4b5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af4b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af4b5-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="af4b5-127">Response</span></span>
<span data-ttu-id="af4b5-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af4b5-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af4b5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="af4b5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="af4b5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4b5-130">Request</span></span>
<span data-ttu-id="af4b5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4b5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="af4b5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4b5-132">Response</span></span>
<span data-ttu-id="af4b5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af4b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "value": [
    {
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
  ]
}
```



