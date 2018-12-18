---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
author: tfitzmac
ms.openlocfilehash: a70a05e965becc15633522b9e38f1ea85fcdea7f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339811"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="8bb96-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8bb96-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="8bb96-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8bb96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bb96-105">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8bb96-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bb96-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8bb96-106">Prerequisites</span></span>
<span data-ttu-id="8bb96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb96-109">Permission type</span></span>|<span data-ttu-id="8bb96-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bb96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bb96-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb96-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8bb96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bb96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb96-114">Not supported.</span></span>|
|<span data-ttu-id="8bb96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bb96-115">Application</span></span>|<span data-ttu-id="8bb96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb96-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bb96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb96-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8bb96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb96-118">Request headers</span></span>
|<span data-ttu-id="8bb96-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bb96-119">Header</span></span>|<span data-ttu-id="8bb96-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8bb96-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bb96-121">Authorization</span></span>|<span data-ttu-id="8bb96-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8bb96-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb96-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8bb96-123">Accept</span></span>|<span data-ttu-id="8bb96-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb96-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb96-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bb96-125">Request body</span></span>
<span data-ttu-id="8bb96-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bb96-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb96-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb96-127">Response</span></span>
<span data-ttu-id="8bb96-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb96-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb96-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb96-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bb96-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb96-130">Request</span></span>
<span data-ttu-id="8bb96-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb96-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="8bb96-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bb96-132">Response</span></span>
<span data-ttu-id="8bb96-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8bb96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

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
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```



