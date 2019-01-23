---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc57c455ae4464ee94e82b0b8ab51b026fdfa129
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418325"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="33e05-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="33e05-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="33e05-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33e05-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33e05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33e05-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33e05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33e05-107">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="33e05-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33e05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="33e05-108">Prerequisites</span></span>
<span data-ttu-id="33e05-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33e05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33e05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33e05-111">Permission type</span></span>|<span data-ttu-id="33e05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33e05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33e05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33e05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33e05-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33e05-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="33e05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33e05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33e05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e05-116">Not supported.</span></span>|
|<span data-ttu-id="33e05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33e05-117">Application</span></span>|<span data-ttu-id="33e05-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33e05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33e05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="33e05-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33e05-120">Request headers</span></span>
|<span data-ttu-id="33e05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33e05-121">Header</span></span>|<span data-ttu-id="33e05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33e05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33e05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33e05-123">Authorization</span></span>|<span data-ttu-id="33e05-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="33e05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33e05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33e05-125">Accept</span></span>|<span data-ttu-id="33e05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33e05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33e05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33e05-127">Request body</span></span>
<span data-ttu-id="33e05-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33e05-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33e05-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="33e05-129">Response</span></span>
<span data-ttu-id="33e05-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="33e05-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33e05-131">Пример</span><span class="sxs-lookup"><span data-stu-id="33e05-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33e05-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33e05-132">Request</span></span>
<span data-ttu-id="33e05-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33e05-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="33e05-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33e05-134">Response</span></span>
<span data-ttu-id="33e05-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="33e05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




