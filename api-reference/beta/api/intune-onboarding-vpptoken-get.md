---
title: Получить vppToken
description: Чтение свойств и связей объекта vppToken.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8fa3ceb27733e30e13f400ece02bac6d937e5d11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849464"
---
# <a name="get-vpptoken"></a><span data-ttu-id="64a4d-103">Получить vppToken</span><span class="sxs-lookup"><span data-stu-id="64a4d-103">Get vppToken</span></span>

> <span data-ttu-id="64a4d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64a4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64a4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64a4d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64a4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64a4d-107">Чтение свойств и связей объекта [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="64a4d-107">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64a4d-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="64a4d-108">Prerequisites</span></span>
<span data-ttu-id="64a4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64a4d-111">Permission type</span></span>|<span data-ttu-id="64a4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64a4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64a4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64a4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64a4d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64a4d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="64a4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64a4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64a4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a4d-116">Not supported.</span></span>|
|<span data-ttu-id="64a4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64a4d-117">Application</span></span>|<span data-ttu-id="64a4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64a4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64a4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64a4d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64a4d-120">Optional query parameters</span></span>
<span data-ttu-id="64a4d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64a4d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64a4d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64a4d-122">Request headers</span></span>
|<span data-ttu-id="64a4d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64a4d-123">Header</span></span>|<span data-ttu-id="64a4d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="64a4d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64a4d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="64a4d-125">Authorization</span></span>|<span data-ttu-id="64a4d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="64a4d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64a4d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="64a4d-127">Accept</span></span>|<span data-ttu-id="64a4d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="64a4d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64a4d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64a4d-129">Request body</span></span>
<span data-ttu-id="64a4d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64a4d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64a4d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="64a4d-131">Response</span></span>
<span data-ttu-id="64a4d-132">В случае успешного выполнения данный метод возвращает`200 OK` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="64a4d-132">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64a4d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="64a4d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="64a4d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="64a4d-134">Request</span></span>
<span data-ttu-id="64a4d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64a4d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="64a4d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="64a4d-136">Response</span></span>
<span data-ttu-id="64a4d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64a4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value",
    "dataSharingConsentGranted": true,
    "displayName": "Display Name value",
    "locationName": "Location Name value",
    "claimTokenManagementFromExternalMdm": true
  }
}
```





