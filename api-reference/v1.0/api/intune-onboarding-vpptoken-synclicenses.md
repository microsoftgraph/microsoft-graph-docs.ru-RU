---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dcd9139bf2d2ca3c7baffbd34fedc064402192f5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759046"
---
# <a name="synclicenses-action"></a><span data-ttu-id="fa203-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="fa203-103">syncLicenses action</span></span>

<span data-ttu-id="fa203-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa203-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa203-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa203-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa203-106">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="fa203-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa203-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="fa203-107">Prerequisites</span></span>
<span data-ttu-id="fa203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa203-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa203-110">Permission type</span></span>|<span data-ttu-id="fa203-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa203-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa203-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa203-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa203-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa203-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa203-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa203-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa203-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa203-115">Not supported.</span></span>|
|<span data-ttu-id="fa203-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa203-116">Application</span></span>|<span data-ttu-id="fa203-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa203-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa203-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa203-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="fa203-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa203-119">Request headers</span></span>
|<span data-ttu-id="fa203-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa203-120">Header</span></span>|<span data-ttu-id="fa203-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa203-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa203-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa203-122">Authorization</span></span>|<span data-ttu-id="fa203-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa203-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa203-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fa203-124">Accept</span></span>|<span data-ttu-id="fa203-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa203-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa203-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa203-126">Request body</span></span>
<span data-ttu-id="fa203-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa203-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa203-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa203-128">Response</span></span>
<span data-ttu-id="fa203-129">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="fa203-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa203-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fa203-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa203-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa203-131">Request</span></span>
<span data-ttu-id="fa203-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa203-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="fa203-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa203-133">Response</span></span>
<span data-ttu-id="fa203-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa203-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




