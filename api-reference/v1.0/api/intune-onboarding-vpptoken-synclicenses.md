---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c81fa85d2b884bc40c580b19635f453645c66af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851046"
---
# <a name="synclicenses-action"></a><span data-ttu-id="84cf6-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="84cf6-103">syncLicenses action</span></span>

> <span data-ttu-id="84cf6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84cf6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84cf6-105">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="84cf6-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84cf6-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="84cf6-106">Prerequisites</span></span>
<span data-ttu-id="84cf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84cf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84cf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84cf6-109">Permission type</span></span>|<span data-ttu-id="84cf6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84cf6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84cf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84cf6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84cf6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84cf6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="84cf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84cf6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84cf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84cf6-114">Not supported.</span></span>|
|<span data-ttu-id="84cf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84cf6-115">Application</span></span>|<span data-ttu-id="84cf6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84cf6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84cf6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84cf6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="84cf6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84cf6-118">Request headers</span></span>
|<span data-ttu-id="84cf6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84cf6-119">Header</span></span>|<span data-ttu-id="84cf6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="84cf6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84cf6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84cf6-121">Authorization</span></span>|<span data-ttu-id="84cf6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84cf6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84cf6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="84cf6-123">Accept</span></span>|<span data-ttu-id="84cf6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84cf6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84cf6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84cf6-125">Request body</span></span>
<span data-ttu-id="84cf6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84cf6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84cf6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="84cf6-127">Response</span></span>
<span data-ttu-id="84cf6-128">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="84cf6-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84cf6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="84cf6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="84cf6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="84cf6-130">Request</span></span>
<span data-ttu-id="84cf6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84cf6-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="84cf6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="84cf6-132">Response</span></span>
<span data-ttu-id="84cf6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84cf6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



