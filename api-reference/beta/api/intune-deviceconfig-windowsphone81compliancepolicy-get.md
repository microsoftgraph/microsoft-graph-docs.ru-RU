---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 985b530ba8349d17b98da876ba0328794bb29c6d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709560"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="4757b-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4757b-103">Get windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="4757b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4757b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4757b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4757b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4757b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4757b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4757b-107">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4757b-107">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4757b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4757b-108">Prerequisites</span></span>
<span data-ttu-id="4757b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4757b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4757b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4757b-111">Permission type</span></span>|<span data-ttu-id="4757b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4757b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4757b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4757b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4757b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4757b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4757b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4757b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4757b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4757b-116">Not supported.</span></span>|
|<span data-ttu-id="4757b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4757b-117">Application</span></span>|<span data-ttu-id="4757b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4757b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4757b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4757b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4757b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4757b-120">Optional query parameters</span></span>
<span data-ttu-id="4757b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4757b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4757b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4757b-122">Request headers</span></span>
|<span data-ttu-id="4757b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4757b-123">Header</span></span>|<span data-ttu-id="4757b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4757b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4757b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4757b-125">Authorization</span></span>|<span data-ttu-id="4757b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4757b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4757b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4757b-127">Accept</span></span>|<span data-ttu-id="4757b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4757b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4757b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4757b-129">Request body</span></span>
<span data-ttu-id="4757b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4757b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4757b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4757b-131">Response</span></span>
<span data-ttu-id="4757b-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4757b-132">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4757b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4757b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4757b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4757b-134">Request</span></span>
<span data-ttu-id="4757b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4757b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4757b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4757b-136">Response</span></span>
<span data-ttu-id="4757b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4757b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





