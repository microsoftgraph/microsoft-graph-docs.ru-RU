---
title: Get mobileAppPolicySetItem
description: Чтение свойств и связей объекта mobileAppPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80079203aaf01123a81f38b32669dba308714230
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159313"
---
# <a name="get-mobileapppolicysetitem"></a><span data-ttu-id="51140-103">Get mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="51140-103">Get mobileAppPolicySetItem</span></span>

<span data-ttu-id="51140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51140-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51140-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51140-107">Чтение свойств и связей объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="51140-107">Read properties and relationships of the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51140-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51140-108">Prerequisites</span></span>
<span data-ttu-id="51140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51140-111">Permission type</span></span>|<span data-ttu-id="51140-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51140-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51140-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51140-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51140-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51140-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51140-116">Not supported.</span></span>|
|<span data-ttu-id="51140-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51140-117">Application</span></span>|<span data-ttu-id="51140-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51140-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51140-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51140-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51140-120">Optional query parameters</span></span>
<span data-ttu-id="51140-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51140-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51140-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51140-122">Request headers</span></span>
|<span data-ttu-id="51140-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51140-123">Header</span></span>|<span data-ttu-id="51140-124">Значение</span><span class="sxs-lookup"><span data-stu-id="51140-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51140-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51140-125">Authorization</span></span>|<span data-ttu-id="51140-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51140-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51140-127">Accept</span><span class="sxs-lookup"><span data-stu-id="51140-127">Accept</span></span>|<span data-ttu-id="51140-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51140-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51140-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51140-129">Request body</span></span>
<span data-ttu-id="51140-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51140-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51140-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="51140-131">Response</span></span>
<span data-ttu-id="51140-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51140-132">If successful, this method returns a `200 OK` response code and [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51140-133">Пример</span><span class="sxs-lookup"><span data-stu-id="51140-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="51140-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="51140-134">Request</span></span>
<span data-ttu-id="51140-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51140-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="51140-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="51140-136">Response</span></span>
<span data-ttu-id="51140-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 769

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
    "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ],
    "intent": "required",
    "settings": {
      "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
      "vpnConfigurationId": "Vpn Configuration Id value",
      "uninstallOnDeviceRemoval": true,
      "isRemovable": true
    }
  }
}
```




