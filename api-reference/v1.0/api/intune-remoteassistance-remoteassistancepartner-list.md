---
title: Список объектов remoteAssistancePartner
description: Список свойств и связей объектов remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b7ac971b1f7638685e1e944bdfb5ed2884aaacf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465870"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="42c0c-103">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="42c0c-103">List remoteAssistancePartners</span></span>

<span data-ttu-id="42c0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42c0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42c0c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42c0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c0c-106">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="42c0c-106">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42c0c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="42c0c-107">Prerequisites</span></span>
<span data-ttu-id="42c0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42c0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42c0c-110">Permission type</span></span>|<span data-ttu-id="42c0c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42c0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42c0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42c0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42c0c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="42c0c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="42c0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42c0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42c0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c0c-115">Not supported.</span></span>|
|<span data-ttu-id="42c0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42c0c-116">Application</span></span>|<span data-ttu-id="42c0c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42c0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42c0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="42c0c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42c0c-119">Request headers</span></span>
|<span data-ttu-id="42c0c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42c0c-120">Header</span></span>|<span data-ttu-id="42c0c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42c0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42c0c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42c0c-122">Authorization</span></span>|<span data-ttu-id="42c0c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42c0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42c0c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42c0c-124">Accept</span></span>|<span data-ttu-id="42c0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42c0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c0c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42c0c-126">Request body</span></span>
<span data-ttu-id="42c0c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42c0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42c0c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="42c0c-128">Response</span></span>
<span data-ttu-id="42c0c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42c0c-129">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c0c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="42c0c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="42c0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42c0c-131">Request</span></span>
<span data-ttu-id="42c0c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42c0c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="42c0c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c0c-133">Response</span></span>
<span data-ttu-id="42c0c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42c0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```






