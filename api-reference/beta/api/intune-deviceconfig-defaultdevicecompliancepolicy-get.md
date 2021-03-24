---
title: Get defaultDeviceCompliancePolicy
description: Чтение свойств и связей объекта defaultDeviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14b3d28382bd92447cf66af467ce7ca3eeeb0b8e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130219"
---
# <a name="get-defaultdevicecompliancepolicy"></a><span data-ttu-id="11afb-103">Get defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="11afb-103">Get defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="11afb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11afb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11afb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11afb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11afb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11afb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11afb-107">Чтение свойств и связей объекта [defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="11afb-107">Read properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11afb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11afb-108">Prerequisites</span></span>
<span data-ttu-id="11afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11afb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11afb-111">Permission type</span></span>|<span data-ttu-id="11afb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11afb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11afb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11afb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11afb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11afb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11afb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11afb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11afb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11afb-116">Not supported.</span></span>|
|<span data-ttu-id="11afb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="11afb-117">Application</span></span>|<span data-ttu-id="11afb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11afb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11afb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11afb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11afb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="11afb-120">Optional query parameters</span></span>
<span data-ttu-id="11afb-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="11afb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11afb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11afb-122">Request headers</span></span>
|<span data-ttu-id="11afb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11afb-123">Header</span></span>|<span data-ttu-id="11afb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="11afb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11afb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="11afb-125">Authorization</span></span>|<span data-ttu-id="11afb-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11afb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11afb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="11afb-127">Accept</span></span>|<span data-ttu-id="11afb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="11afb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11afb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11afb-129">Request body</span></span>
<span data-ttu-id="11afb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11afb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11afb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="11afb-131">Response</span></span>
<span data-ttu-id="11afb-132">В случае успешного использования этот метод возвращает код ответа и `200 OK` [объект defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="11afb-132">If successful, this method returns a `200 OK` response code and [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11afb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="11afb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="11afb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="11afb-134">Request</span></span>
<span data-ttu-id="11afb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11afb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="11afb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="11afb-136">Response</span></span>
<span data-ttu-id="11afb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11afb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a285f027-f027-a285-27f0-85a227f085a2",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




