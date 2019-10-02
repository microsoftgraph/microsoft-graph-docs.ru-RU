---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ccf421c78af50a95829d1af417dbf892bec3b1d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362059"
---
# <a name="synclicenses-action"></a><span data-ttu-id="5517d-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="5517d-103">syncLicenses action</span></span>

> <span data-ttu-id="5517d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5517d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5517d-105">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="5517d-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5517d-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="5517d-106">Prerequisites</span></span>
<span data-ttu-id="5517d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5517d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5517d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5517d-109">Permission type</span></span>|<span data-ttu-id="5517d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5517d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5517d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5517d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5517d-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5517d-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5517d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5517d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5517d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5517d-114">Not supported.</span></span>|
|<span data-ttu-id="5517d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5517d-115">Application</span></span>|<span data-ttu-id="5517d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5517d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5517d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5517d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="5517d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5517d-118">Request headers</span></span>
|<span data-ttu-id="5517d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5517d-119">Header</span></span>|<span data-ttu-id="5517d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5517d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5517d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5517d-121">Authorization</span></span>|<span data-ttu-id="5517d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5517d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5517d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5517d-123">Accept</span></span>|<span data-ttu-id="5517d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5517d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5517d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5517d-125">Request body</span></span>
<span data-ttu-id="5517d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5517d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5517d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5517d-127">Response</span></span>
<span data-ttu-id="5517d-128">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="5517d-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5517d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5517d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5517d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5517d-130">Request</span></span>
<span data-ttu-id="5517d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5517d-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="5517d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5517d-132">Response</span></span>
<span data-ttu-id="5517d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5517d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




