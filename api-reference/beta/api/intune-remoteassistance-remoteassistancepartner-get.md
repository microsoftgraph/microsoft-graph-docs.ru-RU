---
title: Получение remoteAssistancePartner
description: Чтение свойств и связей объекта remoteAssistancePartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f26f97fc57ee5754e718245c18e3bd7430b1c34
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955100"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="76eaa-103">Получение remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="76eaa-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="76eaa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76eaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76eaa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76eaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76eaa-106">Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="76eaa-106">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76eaa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76eaa-107">Prerequisites</span></span>
<span data-ttu-id="76eaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76eaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76eaa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76eaa-110">Permission type</span></span>|<span data-ttu-id="76eaa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76eaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76eaa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76eaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76eaa-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76eaa-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="76eaa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76eaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76eaa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76eaa-115">Not supported.</span></span>|
|<span data-ttu-id="76eaa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76eaa-116">Application</span></span>|<span data-ttu-id="76eaa-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76eaa-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76eaa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76eaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76eaa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76eaa-119">Optional query parameters</span></span>
<span data-ttu-id="76eaa-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76eaa-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76eaa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76eaa-121">Request headers</span></span>
|<span data-ttu-id="76eaa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76eaa-122">Header</span></span>|<span data-ttu-id="76eaa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="76eaa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76eaa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76eaa-124">Authorization</span></span>|<span data-ttu-id="76eaa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76eaa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76eaa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="76eaa-126">Accept</span></span>|<span data-ttu-id="76eaa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="76eaa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76eaa-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76eaa-128">Request body</span></span>
<span data-ttu-id="76eaa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76eaa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76eaa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="76eaa-130">Response</span></span>
<span data-ttu-id="76eaa-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="76eaa-131">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76eaa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="76eaa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="76eaa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="76eaa-133">Request</span></span>
<span data-ttu-id="76eaa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76eaa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="76eaa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="76eaa-135">Response</span></span>
<span data-ttu-id="76eaa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76eaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





