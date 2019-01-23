---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79660c8de56cdf449d3fd407767bed37245ceb2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414279"
---
# <a name="synclicenses-action"></a><span data-ttu-id="ddea5-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="ddea5-103">syncLicenses action</span></span>

> <span data-ttu-id="ddea5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ddea5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ddea5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddea5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddea5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddea5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddea5-107">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="ddea5-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddea5-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="ddea5-108">Prerequisites</span></span>
<span data-ttu-id="ddea5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ddea5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ddea5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddea5-111">Permission type</span></span>|<span data-ttu-id="ddea5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddea5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddea5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddea5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddea5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddea5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ddea5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddea5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddea5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddea5-116">Not supported.</span></span>|
|<span data-ttu-id="ddea5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddea5-117">Application</span></span>|<span data-ttu-id="ddea5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddea5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddea5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddea5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="ddea5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddea5-120">Request headers</span></span>
|<span data-ttu-id="ddea5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddea5-121">Header</span></span>|<span data-ttu-id="ddea5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ddea5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddea5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddea5-123">Authorization</span></span>|<span data-ttu-id="ddea5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ddea5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddea5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddea5-125">Accept</span></span>|<span data-ttu-id="ddea5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddea5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddea5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddea5-127">Request body</span></span>
<span data-ttu-id="ddea5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddea5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddea5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddea5-129">Response</span></span>
<span data-ttu-id="ddea5-130">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="ddea5-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddea5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ddea5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddea5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddea5-132">Request</span></span>
<span data-ttu-id="ddea5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddea5-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="ddea5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddea5-134">Response</span></span>
<span data-ttu-id="ddea5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ddea5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




