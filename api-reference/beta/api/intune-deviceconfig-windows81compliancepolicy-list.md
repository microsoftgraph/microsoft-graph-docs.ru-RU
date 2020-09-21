---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef1764ded01ba24de53021846b44a266dd6d9aeb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086097"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="8ee50-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8ee50-103">List windows81CompliancePolicies</span></span>

<span data-ttu-id="8ee50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ee50-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ee50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ee50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee50-107">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ee50-107">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ee50-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ee50-108">Prerequisites</span></span>
<span data-ttu-id="8ee50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ee50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ee50-111">Permission type</span></span>|<span data-ttu-id="8ee50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ee50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ee50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee50-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ee50-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8ee50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ee50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee50-116">Not supported.</span></span>|
|<span data-ttu-id="8ee50-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ee50-117">Application</span></span>|<span data-ttu-id="8ee50-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ee50-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ee50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8ee50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ee50-120">Request headers</span></span>
|<span data-ttu-id="8ee50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ee50-121">Header</span></span>|<span data-ttu-id="8ee50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ee50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee50-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ee50-123">Authorization</span></span>|<span data-ttu-id="8ee50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ee50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ee50-125">Accept</span></span>|<span data-ttu-id="8ee50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ee50-127">Request body</span></span>
<span data-ttu-id="8ee50-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ee50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ee50-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee50-129">Response</span></span>
<span data-ttu-id="8ee50-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ee50-130">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee50-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8ee50-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ee50-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ee50-132">Request</span></span>
<span data-ttu-id="8ee50-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ee50-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="8ee50-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee50-134">Response</span></span>
<span data-ttu-id="8ee50-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ee50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 953

{
  "value": [
    {
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
  ]
}
```






