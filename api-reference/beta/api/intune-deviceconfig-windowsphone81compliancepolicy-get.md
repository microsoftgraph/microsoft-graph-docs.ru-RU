---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb8f4059679c8d5d67792b28adc5b62ccfde513c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150731"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="760bc-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="760bc-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="760bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="760bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="760bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="760bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760bc-106">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="760bc-106">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="760bc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="760bc-107">Prerequisites</span></span>
<span data-ttu-id="760bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="760bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="760bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="760bc-110">Permission type</span></span>|<span data-ttu-id="760bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="760bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="760bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="760bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="760bc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="760bc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="760bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="760bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="760bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="760bc-115">Not supported.</span></span>|
|<span data-ttu-id="760bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="760bc-116">Application</span></span>|<span data-ttu-id="760bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="760bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="760bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="760bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="760bc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="760bc-119">Optional query parameters</span></span>
<span data-ttu-id="760bc-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="760bc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="760bc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="760bc-121">Request headers</span></span>
|<span data-ttu-id="760bc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="760bc-122">Header</span></span>|<span data-ttu-id="760bc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="760bc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="760bc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="760bc-124">Authorization</span></span>|<span data-ttu-id="760bc-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="760bc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="760bc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="760bc-126">Accept</span></span>|<span data-ttu-id="760bc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="760bc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="760bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="760bc-128">Request body</span></span>
<span data-ttu-id="760bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="760bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="760bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="760bc-130">Response</span></span>
<span data-ttu-id="760bc-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="760bc-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="760bc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="760bc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="760bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="760bc-133">Request</span></span>
<span data-ttu-id="760bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="760bc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="760bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="760bc-135">Response</span></span>
<span data-ttu-id="760bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="760bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```




