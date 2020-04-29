---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1320ef0f5eaa76487d2bb50c98691ea047bfb98
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461998"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="737d6-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="737d6-103">Get windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="737d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="737d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="737d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="737d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="737d6-106">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="737d6-106">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="737d6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="737d6-107">Prerequisites</span></span>
<span data-ttu-id="737d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="737d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="737d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="737d6-110">Permission type</span></span>|<span data-ttu-id="737d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="737d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="737d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="737d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="737d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="737d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="737d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="737d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="737d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737d6-115">Not supported.</span></span>|
|<span data-ttu-id="737d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="737d6-116">Application</span></span>|<span data-ttu-id="737d6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="737d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="737d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="737d6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="737d6-119">Optional query parameters</span></span>
<span data-ttu-id="737d6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="737d6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="737d6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="737d6-121">Request headers</span></span>
|<span data-ttu-id="737d6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="737d6-122">Header</span></span>|<span data-ttu-id="737d6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="737d6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="737d6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="737d6-124">Authorization</span></span>|<span data-ttu-id="737d6-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="737d6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="737d6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="737d6-126">Accept</span></span>|<span data-ttu-id="737d6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="737d6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="737d6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="737d6-128">Request body</span></span>
<span data-ttu-id="737d6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="737d6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="737d6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="737d6-130">Response</span></span>
<span data-ttu-id="737d6-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="737d6-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="737d6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="737d6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="737d6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="737d6-133">Request</span></span>
<span data-ttu-id="737d6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="737d6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="737d6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="737d6-135">Response</span></span>
<span data-ttu-id="737d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="737d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






