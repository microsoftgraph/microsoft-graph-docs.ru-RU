---
title: Список объектов remoteAssistancePartner
description: Список свойств и связей объектов remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6350fd7d519991d8741d2f90350c1b7ee08201
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987029"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="2174b-103">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2174b-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="2174b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2174b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2174b-105">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="2174b-105">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2174b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2174b-106">Prerequisites</span></span>
<span data-ttu-id="2174b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2174b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2174b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2174b-109">Permission type</span></span>|<span data-ttu-id="2174b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2174b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2174b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2174b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2174b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2174b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2174b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2174b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2174b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2174b-114">Not supported.</span></span>|
|<span data-ttu-id="2174b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2174b-115">Application</span></span>|<span data-ttu-id="2174b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2174b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2174b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2174b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="2174b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2174b-118">Request headers</span></span>
|<span data-ttu-id="2174b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2174b-119">Header</span></span>|<span data-ttu-id="2174b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2174b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2174b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2174b-121">Authorization</span></span>|<span data-ttu-id="2174b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2174b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2174b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2174b-123">Accept</span></span>|<span data-ttu-id="2174b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2174b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2174b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2174b-125">Request body</span></span>
<span data-ttu-id="2174b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2174b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2174b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2174b-127">Response</span></span>
<span data-ttu-id="2174b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2174b-128">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2174b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2174b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2174b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2174b-130">Request</span></span>
<span data-ttu-id="2174b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2174b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="2174b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2174b-132">Response</span></span>
<span data-ttu-id="2174b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2174b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



