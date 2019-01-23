---
title: Список объектов remoteAssistancePartner
description: Список свойств и связей объектов remoteAssistancePartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5736f675f0efe93cf601fab4f1a8b8fb033d6a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414776"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="d056a-103">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="d056a-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="d056a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d056a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d056a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d056a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d056a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d056a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d056a-107">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="d056a-107">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d056a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d056a-108">Prerequisites</span></span>
<span data-ttu-id="d056a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d056a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d056a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d056a-111">Permission type</span></span>|<span data-ttu-id="d056a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d056a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d056a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d056a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d056a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d056a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d056a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d056a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d056a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d056a-116">Not supported.</span></span>|
|<span data-ttu-id="d056a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d056a-117">Application</span></span>|<span data-ttu-id="d056a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d056a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d056a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d056a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="d056a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d056a-120">Request headers</span></span>
|<span data-ttu-id="d056a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d056a-121">Header</span></span>|<span data-ttu-id="d056a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d056a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d056a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d056a-123">Authorization</span></span>|<span data-ttu-id="d056a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d056a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d056a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d056a-125">Accept</span></span>|<span data-ttu-id="d056a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d056a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d056a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d056a-127">Request body</span></span>
<span data-ttu-id="d056a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d056a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d056a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d056a-129">Response</span></span>
<span data-ttu-id="d056a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d056a-130">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d056a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d056a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d056a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d056a-132">Request</span></span>
<span data-ttu-id="d056a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d056a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="d056a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d056a-134">Response</span></span>
<span data-ttu-id="d056a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d056a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




