---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 405b4c3596cc16cda1b9b6f9cd4dbf338395290c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980959"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="a727b-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a727b-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="a727b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a727b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a727b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a727b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a727b-106">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="a727b-106">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a727b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a727b-107">Prerequisites</span></span>
<span data-ttu-id="a727b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a727b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a727b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a727b-110">Permission type</span></span>|<span data-ttu-id="a727b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a727b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a727b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a727b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a727b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a727b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a727b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a727b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a727b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a727b-115">Not supported.</span></span>|
|<span data-ttu-id="a727b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a727b-116">Application</span></span>|<span data-ttu-id="a727b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a727b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a727b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a727b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="a727b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a727b-119">Request headers</span></span>
|<span data-ttu-id="a727b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a727b-120">Header</span></span>|<span data-ttu-id="a727b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a727b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a727b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a727b-122">Authorization</span></span>|<span data-ttu-id="a727b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a727b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a727b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a727b-124">Accept</span></span>|<span data-ttu-id="a727b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a727b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a727b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a727b-126">Request body</span></span>
<span data-ttu-id="a727b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a727b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a727b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a727b-128">Response</span></span>
<span data-ttu-id="a727b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a727b-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a727b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a727b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a727b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a727b-131">Request</span></span>
<span data-ttu-id="a727b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a727b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="a727b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a727b-133">Response</span></span>
<span data-ttu-id="a727b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a727b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 794

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```





