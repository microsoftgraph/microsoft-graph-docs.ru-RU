---
title: Список managedDeviceMobileAppConfigurationPolicySetItems
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1e78c3094df462e600e32d3f9f16df4cab9d3ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145140"
---
# <a name="list-manageddevicemobileappconfigurationpolicysetitems"></a><span data-ttu-id="86bbd-103">Список managedDeviceMobileAppConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="86bbd-103">List managedDeviceMobileAppConfigurationPolicySetItems</span></span>

<span data-ttu-id="86bbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86bbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86bbd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86bbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86bbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86bbd-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="86bbd-107">List properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86bbd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86bbd-108">Prerequisites</span></span>
<span data-ttu-id="86bbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86bbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86bbd-111">Permission type</span></span>|<span data-ttu-id="86bbd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86bbd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86bbd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86bbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86bbd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86bbd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86bbd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86bbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86bbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bbd-116">Not supported.</span></span>|
|<span data-ttu-id="86bbd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="86bbd-117">Application</span></span>|<span data-ttu-id="86bbd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86bbd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86bbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86bbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="86bbd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86bbd-120">Request headers</span></span>
|<span data-ttu-id="86bbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86bbd-121">Header</span></span>|<span data-ttu-id="86bbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86bbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86bbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86bbd-123">Authorization</span></span>|<span data-ttu-id="86bbd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86bbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86bbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86bbd-125">Accept</span></span>|<span data-ttu-id="86bbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86bbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86bbd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86bbd-127">Request body</span></span>
<span data-ttu-id="86bbd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86bbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86bbd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="86bbd-129">Response</span></span>
<span data-ttu-id="86bbd-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86bbd-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86bbd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="86bbd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="86bbd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86bbd-132">Request</span></span>
<span data-ttu-id="86bbd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86bbd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="86bbd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="86bbd-134">Response</span></span>
<span data-ttu-id="86bbd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86bbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
      "id": "bb065442-5442-bb06-4254-06bb425406bb",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```




