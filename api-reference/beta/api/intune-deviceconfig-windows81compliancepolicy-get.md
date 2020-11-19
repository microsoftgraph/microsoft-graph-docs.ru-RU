---
title: Получение windows81CompliancePolicy
description: Чтение свойств и связей объекта windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdca63685cbcb7e732201241a115d95d88bc2395
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204441"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="e26f1-103">Получение windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e26f1-103">Get windows81CompliancePolicy</span></span>

<span data-ttu-id="e26f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e26f1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e26f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e26f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e26f1-107">Чтение свойств и связей объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e26f1-107">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e26f1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e26f1-108">Prerequisites</span></span>
<span data-ttu-id="e26f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e26f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e26f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e26f1-111">Permission type</span></span>|<span data-ttu-id="e26f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e26f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e26f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e26f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e26f1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e26f1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e26f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e26f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e26f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26f1-116">Not supported.</span></span>|
|<span data-ttu-id="e26f1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e26f1-117">Application</span></span>|<span data-ttu-id="e26f1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e26f1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e26f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e26f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e26f1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e26f1-120">Optional query parameters</span></span>
<span data-ttu-id="e26f1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e26f1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e26f1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e26f1-122">Request headers</span></span>
|<span data-ttu-id="e26f1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e26f1-123">Header</span></span>|<span data-ttu-id="e26f1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e26f1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e26f1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e26f1-125">Authorization</span></span>|<span data-ttu-id="e26f1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e26f1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e26f1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e26f1-127">Accept</span></span>|<span data-ttu-id="e26f1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e26f1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e26f1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e26f1-129">Request body</span></span>
<span data-ttu-id="e26f1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e26f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e26f1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26f1-131">Response</span></span>
<span data-ttu-id="e26f1-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e26f1-132">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e26f1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e26f1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e26f1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e26f1-134">Request</span></span>
<span data-ttu-id="e26f1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e26f1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="e26f1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26f1-136">Response</span></span>
<span data-ttu-id="e26f1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e26f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
}
```




