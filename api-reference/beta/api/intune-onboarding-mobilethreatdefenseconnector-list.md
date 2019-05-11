---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c8cb3c842de7e1b1b5c8990850132fa6bee5751
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899951"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="5ba8c-103">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="5ba8c-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="5ba8c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ba8c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ba8c-106">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5ba8c-106">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ba8c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5ba8c-107">Prerequisites</span></span>
<span data-ttu-id="5ba8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ba8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ba8c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba8c-110">Permission type</span></span>|<span data-ttu-id="5ba8c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ba8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ba8c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ba8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ba8c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ba8c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5ba8c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ba8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ba8c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-115">Not supported.</span></span>|
|<span data-ttu-id="5ba8c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ba8c-116">Application</span></span>|<span data-ttu-id="5ba8c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ba8c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ba8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5ba8c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ba8c-119">Request headers</span></span>
|<span data-ttu-id="5ba8c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ba8c-120">Header</span></span>|<span data-ttu-id="5ba8c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ba8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ba8c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ba8c-122">Authorization</span></span>|<span data-ttu-id="5ba8c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ba8c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5ba8c-124">Accept</span></span>|<span data-ttu-id="5ba8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ba8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ba8c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ba8c-126">Request body</span></span>
<span data-ttu-id="5ba8c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ba8c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ba8c-128">Response</span></span>
<span data-ttu-id="5ba8c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-129">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ba8c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5ba8c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ba8c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ba8c-131">Request</span></span>
<span data-ttu-id="5ba8c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="5ba8c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ba8c-133">Response</span></span>
<span data-ttu-id="5ba8c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "windowsEnabled": true,
      "macEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "windowsDeviceBlockedOnMissingPartnerData": true,
      "macDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6,
      "allowPartnerToCollectIOSApplicationMetadata": true
    }
  ]
}
```




