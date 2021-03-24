---
title: Получить vppToken
description: Чтение свойств и связей объекта vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba872024e5e34ffb944f593d39d9c70907aedbb9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135000"
---
# <a name="get-vpptoken"></a><span data-ttu-id="43c29-103">Получить vppToken</span><span class="sxs-lookup"><span data-stu-id="43c29-103">Get vppToken</span></span>

<span data-ttu-id="43c29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43c29-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43c29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c29-107">Чтение свойств и связей объекта [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="43c29-107">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c29-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="43c29-108">Prerequisites</span></span>
<span data-ttu-id="43c29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43c29-111">Permission type</span></span>|<span data-ttu-id="43c29-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43c29-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c29-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43c29-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c29-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43c29-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c29-116">Not supported.</span></span>|
|<span data-ttu-id="43c29-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43c29-117">Application</span></span>|<span data-ttu-id="43c29-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c29-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43c29-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43c29-120">Optional query parameters</span></span>
<span data-ttu-id="43c29-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43c29-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43c29-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43c29-122">Request headers</span></span>
|<span data-ttu-id="43c29-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43c29-123">Header</span></span>|<span data-ttu-id="43c29-124">Значение</span><span class="sxs-lookup"><span data-stu-id="43c29-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c29-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c29-125">Authorization</span></span>|<span data-ttu-id="43c29-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43c29-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c29-127">Accept</span><span class="sxs-lookup"><span data-stu-id="43c29-127">Accept</span></span>|<span data-ttu-id="43c29-128">application/json</span><span class="sxs-lookup"><span data-stu-id="43c29-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c29-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43c29-129">Request body</span></span>
<span data-ttu-id="43c29-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43c29-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c29-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c29-131">Response</span></span>
<span data-ttu-id="43c29-132">В случае успешного выполнения данный метод возвращает`200 OK` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="43c29-132">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c29-133">Пример</span><span class="sxs-lookup"><span data-stu-id="43c29-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c29-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="43c29-134">Request</span></span>
<span data-ttu-id="43c29-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43c29-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="43c29-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c29-136">Response</span></span>
<span data-ttu-id="43c29-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43c29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




