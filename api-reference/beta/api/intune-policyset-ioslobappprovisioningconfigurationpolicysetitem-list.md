---
title: Список iosLobAppProvisioningConfigurationPolicySetItems
description: Список свойств и связей объектов iosLobAppProvisioningConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a35506429ab9852f71bef6f8c72c9ceee46ac9d3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156718"
---
# <a name="list-ioslobappprovisioningconfigurationpolicysetitems"></a><span data-ttu-id="3f101-103">Список iosLobAppProvisioningConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="3f101-103">List iosLobAppProvisioningConfigurationPolicySetItems</span></span>

<span data-ttu-id="3f101-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f101-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f101-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f101-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f101-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f101-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f101-107">Список свойств и связей объектов [iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f101-107">List properties and relationships of the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f101-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f101-108">Prerequisites</span></span>
<span data-ttu-id="3f101-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f101-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f101-111">Permission type</span></span>|<span data-ttu-id="3f101-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f101-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f101-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f101-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f101-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f101-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f101-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f101-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f101-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f101-116">Not supported.</span></span>|
|<span data-ttu-id="3f101-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f101-117">Application</span></span>|<span data-ttu-id="3f101-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f101-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f101-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f101-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="3f101-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f101-120">Request headers</span></span>
|<span data-ttu-id="3f101-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f101-121">Header</span></span>|<span data-ttu-id="3f101-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f101-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f101-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f101-123">Authorization</span></span>|<span data-ttu-id="3f101-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f101-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f101-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f101-125">Accept</span></span>|<span data-ttu-id="3f101-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f101-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f101-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f101-127">Request body</span></span>
<span data-ttu-id="3f101-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f101-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f101-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f101-129">Response</span></span>
<span data-ttu-id="3f101-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3f101-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f101-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3f101-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f101-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f101-132">Request</span></span>
<span data-ttu-id="3f101-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f101-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="3f101-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f101-134">Response</span></span>
<span data-ttu-id="3f101-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f101-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
      "id": "6a978d58-8d58-6a97-588d-976a588d976a",
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




