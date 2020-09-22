---
title: Список объектов remoteAssistancePartner
description: Список свойств и связей объектов remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d552dabb72ae748dda32c2a490fb885d21d9e665
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010873"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="5bd04-103">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5bd04-103">List remoteAssistancePartners</span></span>

<span data-ttu-id="5bd04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bd04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bd04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bd04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bd04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bd04-107">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="5bd04-107">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bd04-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5bd04-108">Prerequisites</span></span>
<span data-ttu-id="5bd04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bd04-111">Permission type</span></span>|<span data-ttu-id="5bd04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bd04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bd04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5bd04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bd04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd04-116">Not supported.</span></span>|
|<span data-ttu-id="5bd04-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5bd04-117">Application</span></span>|<span data-ttu-id="5bd04-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd04-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bd04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="5bd04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5bd04-120">Request headers</span></span>
|<span data-ttu-id="5bd04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bd04-121">Header</span></span>|<span data-ttu-id="5bd04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5bd04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd04-123">Authorization</span></span>|<span data-ttu-id="5bd04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bd04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5bd04-125">Accept</span></span>|<span data-ttu-id="5bd04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bd04-127">Request body</span></span>
<span data-ttu-id="5bd04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bd04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bd04-129">Response</span></span>
<span data-ttu-id="5bd04-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5bd04-130">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5bd04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bd04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bd04-132">Request</span></span>
<span data-ttu-id="5bd04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bd04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="5bd04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bd04-134">Response</span></span>
<span data-ttu-id="5bd04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bd04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
    }
  ]
}
```






