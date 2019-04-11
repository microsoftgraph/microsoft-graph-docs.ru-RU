---
title: Получение deviceManagementPartner
description: Чтение свойств и связей объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a816615074709bec7b60b7aa27d1ebfc1f1e601
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783642"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="da633-103">Получение deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="da633-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="da633-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da633-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da633-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da633-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da633-106">Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="da633-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da633-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="da633-107">Prerequisites</span></span>
<span data-ttu-id="da633-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da633-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da633-110">Permission type</span></span>|<span data-ttu-id="da633-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da633-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da633-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da633-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da633-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da633-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="da633-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da633-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da633-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da633-115">Not supported.</span></span>|
|<span data-ttu-id="da633-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da633-116">Application</span></span>|<span data-ttu-id="da633-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da633-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da633-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da633-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da633-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da633-119">Optional query parameters</span></span>
<span data-ttu-id="da633-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da633-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da633-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da633-121">Request headers</span></span>
|<span data-ttu-id="da633-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da633-122">Header</span></span>|<span data-ttu-id="da633-123">Значение</span><span class="sxs-lookup"><span data-stu-id="da633-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da633-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da633-124">Authorization</span></span>|<span data-ttu-id="da633-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da633-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da633-126">Accept</span><span class="sxs-lookup"><span data-stu-id="da633-126">Accept</span></span>|<span data-ttu-id="da633-127">application/json</span><span class="sxs-lookup"><span data-stu-id="da633-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da633-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da633-128">Request body</span></span>
<span data-ttu-id="da633-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da633-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da633-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="da633-130">Response</span></span>
<span data-ttu-id="da633-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da633-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da633-132">Пример</span><span class="sxs-lookup"><span data-stu-id="da633-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="da633-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="da633-133">Request</span></span>
<span data-ttu-id="da633-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da633-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="da633-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="da633-135">Response</span></span>
<span data-ttu-id="da633-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da633-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
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
}
```





