---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
author: tfitzmac
ms.openlocfilehash: 5a950aadd1ca05892c9092cf6a7b9d2262ed0f72
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333782"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="71bbf-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="71bbf-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="71bbf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71bbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71bbf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71bbf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71bbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71bbf-107">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="71bbf-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71bbf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71bbf-108">Prerequisites</span></span>
<span data-ttu-id="71bbf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71bbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71bbf-111">Permission type</span></span>|<span data-ttu-id="71bbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71bbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71bbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71bbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71bbf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71bbf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="71bbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71bbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bbf-116">Not supported.</span></span>|
|<span data-ttu-id="71bbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71bbf-117">Application</span></span>|<span data-ttu-id="71bbf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71bbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71bbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="71bbf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71bbf-120">Request headers</span></span>
|<span data-ttu-id="71bbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71bbf-121">Header</span></span>|<span data-ttu-id="71bbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71bbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71bbf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71bbf-123">Authorization</span></span>|<span data-ttu-id="71bbf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71bbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71bbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71bbf-125">Accept</span></span>|<span data-ttu-id="71bbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71bbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71bbf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71bbf-127">Request body</span></span>
<span data-ttu-id="71bbf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71bbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71bbf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71bbf-129">Response</span></span>
<span data-ttu-id="71bbf-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71bbf-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71bbf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71bbf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="71bbf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71bbf-132">Request</span></span>
<span data-ttu-id="71bbf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71bbf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="71bbf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="71bbf-134">Response</span></span>
<span data-ttu-id="71bbf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71bbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





