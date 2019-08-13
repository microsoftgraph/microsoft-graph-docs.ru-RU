---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb03c5de29892de1854e1c5678e9bb54cf69d628
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352261"
---
# <a name="synclicenses-action"></a><span data-ttu-id="bdeea-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="bdeea-103">syncLicenses action</span></span>

> <span data-ttu-id="bdeea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdeea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdeea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdeea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdeea-106">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="bdeea-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdeea-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="bdeea-107">Prerequisites</span></span>
<span data-ttu-id="bdeea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdeea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdeea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdeea-110">Permission type</span></span>|<span data-ttu-id="bdeea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdeea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdeea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdeea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdeea-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdeea-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bdeea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdeea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdeea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdeea-115">Not supported.</span></span>|
|<span data-ttu-id="bdeea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdeea-116">Application</span></span>|<span data-ttu-id="bdeea-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdeea-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdeea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdeea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bdeea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdeea-119">Request headers</span></span>
|<span data-ttu-id="bdeea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdeea-120">Header</span></span>|<span data-ttu-id="bdeea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bdeea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdeea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdeea-122">Authorization</span></span>|<span data-ttu-id="bdeea-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdeea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdeea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bdeea-124">Accept</span></span>|<span data-ttu-id="bdeea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdeea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdeea-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdeea-126">Request body</span></span>
<span data-ttu-id="bdeea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdeea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdeea-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdeea-128">Response</span></span>
<span data-ttu-id="bdeea-129">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="bdeea-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdeea-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bdeea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdeea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdeea-131">Request</span></span>
<span data-ttu-id="bdeea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdeea-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="bdeea-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdeea-133">Response</span></span>
<span data-ttu-id="bdeea-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdeea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






