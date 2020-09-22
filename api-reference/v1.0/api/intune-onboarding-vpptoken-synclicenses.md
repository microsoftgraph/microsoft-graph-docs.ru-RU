---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03129a7db4975614605461d4211539e49bdd7cf7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997342"
---
# <a name="synclicenses-action"></a><span data-ttu-id="36753-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="36753-103">syncLicenses action</span></span>

<span data-ttu-id="36753-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36753-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36753-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36753-106">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="36753-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36753-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="36753-107">Prerequisites</span></span>
<span data-ttu-id="36753-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36753-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36753-110">Permission type</span></span>|<span data-ttu-id="36753-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36753-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36753-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36753-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36753-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36753-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36753-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36753-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36753-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36753-115">Not supported.</span></span>|
|<span data-ttu-id="36753-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36753-116">Application</span></span>|<span data-ttu-id="36753-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36753-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36753-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36753-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="36753-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36753-119">Request headers</span></span>
|<span data-ttu-id="36753-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36753-120">Header</span></span>|<span data-ttu-id="36753-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36753-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36753-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36753-122">Authorization</span></span>|<span data-ttu-id="36753-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36753-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36753-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36753-124">Accept</span></span>|<span data-ttu-id="36753-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36753-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36753-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36753-126">Request body</span></span>
<span data-ttu-id="36753-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36753-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36753-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36753-128">Response</span></span>
<span data-ttu-id="36753-129">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="36753-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36753-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36753-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="36753-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36753-131">Request</span></span>
<span data-ttu-id="36753-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36753-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="36753-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="36753-133">Response</span></span>
<span data-ttu-id="36753-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36753-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









