---
title: Получение iosLobAppProvisioningConfiguration
description: Чтение свойства и связи объекта iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f92ae8f7054e9a7be87fd7891d2468f345f389a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914572"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c9d4b-103">Получение iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9d4b-103">Get iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="c9d4b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9d4b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9d4b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9d4b-107">Чтение свойства и связи объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c9d4b-107">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9d4b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9d4b-108">Prerequisites</span></span>
<span data-ttu-id="c9d4b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d4b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d4b-111">Permission type</span></span>|<span data-ttu-id="c9d4b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9d4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9d4b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9d4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9d4b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9d4b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c9d4b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9d4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9d4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-116">Not supported.</span></span>|
|<span data-ttu-id="c9d4b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9d4b-117">Application</span></span>|<span data-ttu-id="c9d4b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9d4b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9d4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9d4b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9d4b-120">Optional query parameters</span></span>
<span data-ttu-id="c9d4b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9d4b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9d4b-122">Request headers</span></span>
|<span data-ttu-id="c9d4b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9d4b-123">Header</span></span>|<span data-ttu-id="c9d4b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c9d4b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9d4b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9d4b-125">Authorization</span></span>|<span data-ttu-id="c9d4b-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c9d4b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9d4b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c9d4b-127">Accept</span></span>|<span data-ttu-id="c9d4b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c9d4b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9d4b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9d4b-129">Request body</span></span>
<span data-ttu-id="c9d4b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9d4b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9d4b-131">Response</span></span>
<span data-ttu-id="c9d4b-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d4b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c9d4b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9d4b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9d4b-134">Request</span></span>
<span data-ttu-id="c9d4b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c9d4b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9d4b-136">Response</span></span>
<span data-ttu-id="c9d4b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c9d4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
    "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```





