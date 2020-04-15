---
title: Список VPP токенов
description: Список свойств и связей объектов VPP токены.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a68702c01dafd0931c429039e3519782abf9ff9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452814"
---
# <a name="list-vpptokens"></a><span data-ttu-id="b5b42-103">Список VPP токенов</span><span class="sxs-lookup"><span data-stu-id="b5b42-103">List vppTokens</span></span>

<span data-ttu-id="b5b42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5b42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5b42-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5b42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5b42-106">Список свойств и связей объектов [VPP токены](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="b5b42-106">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5b42-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="b5b42-107">Prerequisites</span></span>
<span data-ttu-id="b5b42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5b42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5b42-110">Permission type</span></span>|<span data-ttu-id="b5b42-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5b42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5b42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5b42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5b42-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5b42-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b5b42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5b42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5b42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5b42-115">Not supported.</span></span>|
|<span data-ttu-id="b5b42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5b42-116">Application</span></span>|<span data-ttu-id="b5b42-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5b42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5b42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5b42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="b5b42-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5b42-119">Request headers</span></span>
|<span data-ttu-id="b5b42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5b42-120">Header</span></span>|<span data-ttu-id="b5b42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5b42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5b42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b42-122">Authorization</span></span>|<span data-ttu-id="b5b42-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5b42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5b42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5b42-124">Accept</span></span>|<span data-ttu-id="b5b42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5b42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5b42-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5b42-126">Request body</span></span>
<span data-ttu-id="b5b42-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5b42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5b42-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5b42-128">Response</span></span>
<span data-ttu-id="b5b42-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [VPP Токенов ](../resources/intune-onboarding-vpptoken.md) в текстовом поле для отклика.</span><span class="sxs-lookup"><span data-stu-id="b5b42-129">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b42-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b5b42-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5b42-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5b42-131">Request</span></span>
<span data-ttu-id="b5b42-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5b42-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="b5b42-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5b42-133">Response</span></span>
<span data-ttu-id="b5b42-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5b42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
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
  ]
}
```






