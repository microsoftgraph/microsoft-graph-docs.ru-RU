---
title: Получить vppToken
description: Чтение свойств и связей объекта vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46031be0db458c845d862db75fc7b88405dd050f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708020"
---
# <a name="get-vpptoken"></a><span data-ttu-id="2d514-103">Получить vppToken</span><span class="sxs-lookup"><span data-stu-id="2d514-103">Get vppToken</span></span>

<span data-ttu-id="2d514-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d514-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d514-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d514-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d514-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d514-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d514-107">Чтение свойств и связей объекта [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="2d514-107">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d514-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="2d514-108">Prerequisites</span></span>
<span data-ttu-id="2d514-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d514-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d514-111">Permission type</span></span>|<span data-ttu-id="2d514-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d514-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d514-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d514-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d514-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d514-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2d514-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d514-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d514-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d514-116">Not supported.</span></span>|
|<span data-ttu-id="2d514-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d514-117">Application</span></span>|<span data-ttu-id="2d514-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d514-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d514-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d514-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d514-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d514-120">Optional query parameters</span></span>
<span data-ttu-id="2d514-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2d514-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d514-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d514-122">Request headers</span></span>
|<span data-ttu-id="2d514-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d514-123">Header</span></span>|<span data-ttu-id="2d514-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2d514-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d514-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d514-125">Authorization</span></span>|<span data-ttu-id="2d514-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d514-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d514-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2d514-127">Accept</span></span>|<span data-ttu-id="2d514-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2d514-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d514-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d514-129">Request body</span></span>
<span data-ttu-id="2d514-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d514-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d514-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d514-131">Response</span></span>
<span data-ttu-id="2d514-132">В случае успешного выполнения данный метод возвращает`200 OK` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="2d514-132">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d514-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2d514-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d514-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d514-134">Request</span></span>
<span data-ttu-id="2d514-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d514-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="2d514-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d514-136">Response</span></span>
<span data-ttu-id="2d514-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d514-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





