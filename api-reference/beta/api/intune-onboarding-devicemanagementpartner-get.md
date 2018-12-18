---
title: Получение deviceManagementPartner
description: Чтение свойств и связей объекта deviceManagementPartner.
author: tfitzmac
ms.openlocfilehash: cb37c12f2624ff31d3346aaa525202a6919b50c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351865"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="00ceb-103">Получение deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="00ceb-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="00ceb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00ceb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ceb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00ceb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00ceb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00ceb-107">Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="00ceb-107">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00ceb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00ceb-108">Prerequisites</span></span>
<span data-ttu-id="00ceb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ceb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00ceb-111">Permission type</span></span>|<span data-ttu-id="00ceb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00ceb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00ceb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00ceb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00ceb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="00ceb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="00ceb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00ceb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00ceb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ceb-116">Not supported.</span></span>|
|<span data-ttu-id="00ceb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00ceb-117">Application</span></span>|<span data-ttu-id="00ceb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ceb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00ceb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00ceb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00ceb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00ceb-120">Optional query parameters</span></span>
<span data-ttu-id="00ceb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00ceb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00ceb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00ceb-122">Request headers</span></span>
|<span data-ttu-id="00ceb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00ceb-123">Header</span></span>|<span data-ttu-id="00ceb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="00ceb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00ceb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00ceb-125">Authorization</span></span>|<span data-ttu-id="00ceb-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00ceb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00ceb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="00ceb-127">Accept</span></span>|<span data-ttu-id="00ceb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="00ceb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ceb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00ceb-129">Request body</span></span>
<span data-ttu-id="00ceb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00ceb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00ceb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ceb-131">Response</span></span>
<span data-ttu-id="00ceb-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00ceb-132">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ceb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="00ceb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="00ceb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ceb-134">Request</span></span>
<span data-ttu-id="00ceb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00ceb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="00ceb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="00ceb-136">Response</span></span>
<span data-ttu-id="00ceb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00ceb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





