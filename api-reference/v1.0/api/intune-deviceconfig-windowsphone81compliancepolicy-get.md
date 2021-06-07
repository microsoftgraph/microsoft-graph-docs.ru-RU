---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 069b553a34f186237da5fce0886e22cc2f47ccfe
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747139"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="8bafa-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8bafa-103">Get windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="8bafa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bafa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bafa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bafa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bafa-106">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8bafa-106">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bafa-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8bafa-107">Prerequisites</span></span>
<span data-ttu-id="8bafa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bafa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bafa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bafa-110">Permission type</span></span>|<span data-ttu-id="8bafa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bafa-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bafa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bafa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bafa-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bafa-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bafa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bafa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bafa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bafa-115">Not supported.</span></span>|
|<span data-ttu-id="8bafa-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8bafa-116">Application</span></span>|<span data-ttu-id="8bafa-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bafa-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bafa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bafa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bafa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8bafa-119">Optional query parameters</span></span>
<span data-ttu-id="8bafa-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8bafa-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bafa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bafa-121">Request headers</span></span>
|<span data-ttu-id="8bafa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bafa-122">Header</span></span>|<span data-ttu-id="8bafa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8bafa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bafa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bafa-124">Authorization</span></span>|<span data-ttu-id="8bafa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bafa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bafa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8bafa-126">Accept</span></span>|<span data-ttu-id="8bafa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8bafa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bafa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bafa-128">Request body</span></span>
<span data-ttu-id="8bafa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bafa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bafa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bafa-130">Response</span></span>
<span data-ttu-id="8bafa-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8bafa-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bafa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8bafa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bafa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bafa-133">Request</span></span>
<span data-ttu-id="8bafa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bafa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="8bafa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bafa-135">Response</span></span>
<span data-ttu-id="8bafa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bafa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




