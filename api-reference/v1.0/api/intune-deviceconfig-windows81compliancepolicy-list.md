---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
ms.openlocfilehash: b167d1d890820598d31bcfd5d6abf56dc256f2c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027549"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="5a964-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5a964-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="5a964-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a964-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a964-105">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5a964-105">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a964-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5a964-106">Prerequisites</span></span>
<span data-ttu-id="5a964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a964-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a964-109">Permission type</span></span>|<span data-ttu-id="5a964-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a964-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a964-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a964-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a964-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a964-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a964-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a964-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a964-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a964-114">Not supported.</span></span>|
|<span data-ttu-id="5a964-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a964-115">Application</span></span>|<span data-ttu-id="5a964-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a964-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a964-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a964-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5a964-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a964-118">Request headers</span></span>
|<span data-ttu-id="5a964-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a964-119">Header</span></span>|<span data-ttu-id="5a964-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5a964-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a964-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a964-121">Authorization</span></span>|<span data-ttu-id="5a964-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5a964-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a964-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5a964-123">Accept</span></span>|<span data-ttu-id="5a964-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a964-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a964-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a964-125">Request body</span></span>
<span data-ttu-id="5a964-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a964-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a964-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a964-127">Response</span></span>
<span data-ttu-id="5a964-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a964-128">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a964-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5a964-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a964-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a964-130">Request</span></span>
<span data-ttu-id="5a964-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a964-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="5a964-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a964-132">Response</span></span>
<span data-ttu-id="5a964-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5a964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



