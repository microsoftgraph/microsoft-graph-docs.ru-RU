---
title: Получить vppToken
description: Чтение свойств и связей объекта vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ab5fce07679dbfdacb22d62e59b08f8b9febe54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023960"
---
# <a name="get-vpptoken"></a><span data-ttu-id="ef9de-103">Получить vppToken</span><span class="sxs-lookup"><span data-stu-id="ef9de-103">Get vppToken</span></span>

> <span data-ttu-id="ef9de-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef9de-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef9de-105">Чтение свойств и связей объекта [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="ef9de-105">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef9de-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="ef9de-106">Prerequisites</span></span>
<span data-ttu-id="ef9de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef9de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef9de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9de-109">Permission type</span></span>|<span data-ttu-id="ef9de-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef9de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef9de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9de-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef9de-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ef9de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef9de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9de-114">Not supported.</span></span>|
|<span data-ttu-id="ef9de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef9de-115">Application</span></span>|<span data-ttu-id="ef9de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef9de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef9de-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef9de-118">Optional query parameters</span></span>
<span data-ttu-id="ef9de-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9de-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef9de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef9de-120">Request headers</span></span>
|<span data-ttu-id="ef9de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef9de-121">Header</span></span>|<span data-ttu-id="ef9de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef9de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef9de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef9de-123">Authorization</span></span>|<span data-ttu-id="ef9de-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef9de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef9de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef9de-125">Accept</span></span>|<span data-ttu-id="ef9de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef9de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef9de-127">Request body</span></span>
<span data-ttu-id="ef9de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef9de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef9de-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef9de-129">Response</span></span>
<span data-ttu-id="ef9de-130">В случае успешного выполнения данный метод возвращает`200 OK` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="ef9de-130">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef9de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ef9de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef9de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef9de-132">Request</span></span>
<span data-ttu-id="ef9de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef9de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="ef9de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef9de-134">Response</span></span>
<span data-ttu-id="ef9de-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef9de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



