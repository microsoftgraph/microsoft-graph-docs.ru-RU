---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a7729ed08cb21b46577d6644bbead87aeda4f2f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42737395"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="64a7b-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="64a7b-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="64a7b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64a7b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64a7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64a7b-106">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="64a7b-106">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64a7b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64a7b-107">Prerequisites</span></span>
<span data-ttu-id="64a7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a7b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64a7b-110">Permission type</span></span>|<span data-ttu-id="64a7b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64a7b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64a7b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64a7b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64a7b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64a7b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64a7b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64a7b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64a7b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a7b-115">Not supported.</span></span>|
|<span data-ttu-id="64a7b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="64a7b-116">Application</span></span>|<span data-ttu-id="64a7b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64a7b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64a7b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64a7b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="64a7b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64a7b-119">Request headers</span></span>
|<span data-ttu-id="64a7b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64a7b-120">Header</span></span>|<span data-ttu-id="64a7b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64a7b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64a7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64a7b-122">Authorization</span></span>|<span data-ttu-id="64a7b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64a7b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64a7b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64a7b-124">Accept</span></span>|<span data-ttu-id="64a7b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64a7b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64a7b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64a7b-126">Request body</span></span>
<span data-ttu-id="64a7b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64a7b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64a7b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="64a7b-128">Response</span></span>
<span data-ttu-id="64a7b-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64a7b-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64a7b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="64a7b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64a7b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="64a7b-131">Request</span></span>
<span data-ttu-id="64a7b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64a7b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="64a7b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64a7b-133">Response</span></span>
<span data-ttu-id="64a7b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64a7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




