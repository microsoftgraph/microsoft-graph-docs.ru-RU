---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a6e6aaed7260754ca1a9e5da9bd90b24a2519a9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933143"
---
# <a name="synclicenses-action"></a><span data-ttu-id="734ed-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="734ed-103">syncLicenses action</span></span>

> <span data-ttu-id="734ed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="734ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="734ed-105">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="734ed-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="734ed-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="734ed-106">Prerequisites</span></span>
<span data-ttu-id="734ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="734ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="734ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="734ed-109">Permission type</span></span>|<span data-ttu-id="734ed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="734ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="734ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="734ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="734ed-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734ed-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="734ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="734ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="734ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="734ed-114">Not supported.</span></span>|
|<span data-ttu-id="734ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="734ed-115">Application</span></span>|<span data-ttu-id="734ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="734ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="734ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="734ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="734ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="734ed-118">Request headers</span></span>
|<span data-ttu-id="734ed-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="734ed-119">Header</span></span>|<span data-ttu-id="734ed-120">Значение</span><span class="sxs-lookup"><span data-stu-id="734ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="734ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="734ed-121">Authorization</span></span>|<span data-ttu-id="734ed-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="734ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="734ed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="734ed-123">Accept</span></span>|<span data-ttu-id="734ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="734ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="734ed-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="734ed-125">Request body</span></span>
<span data-ttu-id="734ed-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="734ed-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="734ed-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="734ed-127">Response</span></span>
<span data-ttu-id="734ed-128">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="734ed-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="734ed-129">Пример</span><span class="sxs-lookup"><span data-stu-id="734ed-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="734ed-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="734ed-130">Request</span></span>
<span data-ttu-id="734ed-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="734ed-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="734ed-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="734ed-132">Response</span></span>
<span data-ttu-id="734ed-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="734ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

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
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```



