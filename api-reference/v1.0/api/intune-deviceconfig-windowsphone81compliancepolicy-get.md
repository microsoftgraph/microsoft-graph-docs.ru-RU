---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 089f8a826620faa961e8304a2c7e54bdb77d6d11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018864"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="4b227-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4b227-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="4b227-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b227-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b227-105">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b227-105">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b227-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4b227-106">Prerequisites</span></span>
<span data-ttu-id="4b227-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b227-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b227-109">Permission type</span></span>|<span data-ttu-id="4b227-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b227-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b227-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b227-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b227-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b227-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b227-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b227-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b227-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b227-114">Not supported.</span></span>|
|<span data-ttu-id="4b227-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b227-115">Application</span></span>|<span data-ttu-id="4b227-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b227-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b227-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b227-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b227-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b227-118">Optional query parameters</span></span>
<span data-ttu-id="4b227-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b227-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b227-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b227-120">Request headers</span></span>
|<span data-ttu-id="4b227-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b227-121">Header</span></span>|<span data-ttu-id="4b227-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b227-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b227-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b227-123">Authorization</span></span>|<span data-ttu-id="4b227-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b227-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b227-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b227-125">Accept</span></span>|<span data-ttu-id="4b227-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b227-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b227-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b227-127">Request body</span></span>
<span data-ttu-id="4b227-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b227-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b227-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b227-129">Response</span></span>
<span data-ttu-id="4b227-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b227-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b227-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4b227-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b227-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b227-132">Request</span></span>
<span data-ttu-id="4b227-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b227-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4b227-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b227-134">Response</span></span>
<span data-ttu-id="4b227-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b227-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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



