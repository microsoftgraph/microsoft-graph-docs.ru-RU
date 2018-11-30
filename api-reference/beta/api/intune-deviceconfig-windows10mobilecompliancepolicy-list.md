---
title: Перечисление объектов windows10MobileCompliancePolicy
description: Список свойств и связей объектов windows10MobileCompliancePolicy.
ms.openlocfilehash: fe86eb61a578fb22ed1f471ca7b2b518bb440667
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077786"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="8cf1d-103">Перечисление объектов windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8cf1d-103">List windows10MobileCompliancePolicies</span></span>

> <span data-ttu-id="8cf1d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cf1d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cf1d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cf1d-107">Список свойств и связей объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8cf1d-107">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cf1d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8cf1d-108">Prerequisites</span></span>
<span data-ttu-id="8cf1d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf1d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cf1d-111">Permission type</span></span>|<span data-ttu-id="8cf1d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cf1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cf1d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cf1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cf1d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cf1d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8cf1d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cf1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cf1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-116">Not supported.</span></span>|
|<span data-ttu-id="8cf1d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cf1d-117">Application</span></span>|<span data-ttu-id="8cf1d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cf1d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cf1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8cf1d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cf1d-120">Request headers</span></span>
|<span data-ttu-id="8cf1d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cf1d-121">Header</span></span>|<span data-ttu-id="8cf1d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cf1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cf1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf1d-123">Authorization</span></span>|<span data-ttu-id="8cf1d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8cf1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cf1d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cf1d-125">Accept</span></span>|<span data-ttu-id="8cf1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cf1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cf1d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cf1d-127">Request body</span></span>
<span data-ttu-id="8cf1d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cf1d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cf1d-129">Response</span></span>
<span data-ttu-id="8cf1d-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-130">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf1d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8cf1d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cf1d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cf1d-132">Request</span></span>
<span data-ttu-id="8cf1d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cf1d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="8cf1d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cf1d-134">Response</span></span>
<span data-ttu-id="8cf1d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8cf1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ]
    }
  ]
}
```





