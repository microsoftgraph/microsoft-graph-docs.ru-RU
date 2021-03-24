---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343474868b0ae0978704186ce0ec3bd14de622a1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134986"
---
# <a name="synclicenses-action"></a><span data-ttu-id="9d1ad-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="9d1ad-103">syncLicenses action</span></span>

<span data-ttu-id="9d1ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d1ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d1ad-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d1ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d1ad-107">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="9d1ad-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d1ad-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="9d1ad-108">Prerequisites</span></span>
<span data-ttu-id="9d1ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d1ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d1ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d1ad-111">Permission type</span></span>|<span data-ttu-id="9d1ad-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d1ad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d1ad-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d1ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d1ad-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d1ad-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9d1ad-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d1ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d1ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-116">Not supported.</span></span>|
|<span data-ttu-id="9d1ad-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9d1ad-117">Application</span></span>|<span data-ttu-id="9d1ad-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d1ad-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d1ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d1ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="9d1ad-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d1ad-120">Request headers</span></span>
|<span data-ttu-id="9d1ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d1ad-121">Header</span></span>|<span data-ttu-id="9d1ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d1ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d1ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d1ad-123">Authorization</span></span>|<span data-ttu-id="9d1ad-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d1ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d1ad-125">Accept</span></span>|<span data-ttu-id="9d1ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d1ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d1ad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d1ad-127">Request body</span></span>
<span data-ttu-id="9d1ad-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d1ad-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d1ad-129">Response</span></span>
<span data-ttu-id="9d1ad-130">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d1ad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9d1ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d1ad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d1ad-132">Request</span></span>
<span data-ttu-id="9d1ad-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="9d1ad-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d1ad-134">Response</span></span>
<span data-ttu-id="9d1ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d1ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

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
    "claimTokenManagementFromExternalMdm": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




