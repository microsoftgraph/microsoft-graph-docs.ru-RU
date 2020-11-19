---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5194165cb6760e2fb3fddc7ae703a7f9938b755f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211462"
---
# <a name="synclicenses-action"></a><span data-ttu-id="3d637-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="3d637-103">syncLicenses action</span></span>

<span data-ttu-id="3d637-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d637-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d637-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d637-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d637-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d637-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d637-107">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="3d637-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d637-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="3d637-108">Prerequisites</span></span>
<span data-ttu-id="3d637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d637-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d637-111">Permission type</span></span>|<span data-ttu-id="3d637-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d637-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d637-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d637-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d637-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d637-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d637-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d637-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d637-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d637-116">Not supported.</span></span>|
|<span data-ttu-id="3d637-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d637-117">Application</span></span>|<span data-ttu-id="3d637-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d637-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d637-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d637-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="3d637-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d637-120">Request headers</span></span>
|<span data-ttu-id="3d637-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d637-121">Header</span></span>|<span data-ttu-id="3d637-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d637-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d637-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d637-123">Authorization</span></span>|<span data-ttu-id="3d637-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d637-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d637-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d637-125">Accept</span></span>|<span data-ttu-id="3d637-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d637-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d637-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d637-127">Request body</span></span>
<span data-ttu-id="3d637-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d637-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d637-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d637-129">Response</span></span>
<span data-ttu-id="3d637-130">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="3d637-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d637-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3d637-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d637-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d637-132">Request</span></span>
<span data-ttu-id="3d637-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d637-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="3d637-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d637-134">Response</span></span>
<span data-ttu-id="3d637-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d637-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




