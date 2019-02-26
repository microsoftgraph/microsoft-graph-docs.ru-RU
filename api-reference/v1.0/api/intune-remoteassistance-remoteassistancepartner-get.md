---
title: Получение remoteAssistancePartner
description: Чтение свойств и связей объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a796cf6ca84e3364bb2322d846bae2ccf57e754
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262834"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="091c4-103">Получение remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="091c4-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="091c4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="091c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="091c4-105">Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="091c4-105">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="091c4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="091c4-106">Prerequisites</span></span>
<span data-ttu-id="091c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="091c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="091c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="091c4-109">Permission type</span></span>|<span data-ttu-id="091c4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="091c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="091c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="091c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="091c4-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="091c4-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="091c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="091c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="091c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091c4-114">Not supported.</span></span>|
|<span data-ttu-id="091c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="091c4-115">Application</span></span>|<span data-ttu-id="091c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="091c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="091c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="091c4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="091c4-118">Optional query parameters</span></span>
<span data-ttu-id="091c4-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="091c4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="091c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="091c4-120">Request headers</span></span>
|<span data-ttu-id="091c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="091c4-121">Header</span></span>|<span data-ttu-id="091c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="091c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="091c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="091c4-123">Authorization</span></span>|<span data-ttu-id="091c4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="091c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="091c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="091c4-125">Accept</span></span>|<span data-ttu-id="091c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="091c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="091c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="091c4-127">Request body</span></span>
<span data-ttu-id="091c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="091c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="091c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="091c4-129">Response</span></span>
<span data-ttu-id="091c4-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="091c4-130">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="091c4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="091c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="091c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="091c4-132">Request</span></span>
<span data-ttu-id="091c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="091c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="091c4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="091c4-134">Response</span></span>
<span data-ttu-id="091c4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="091c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



