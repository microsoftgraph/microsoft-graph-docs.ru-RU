---
title: Получение объекта androidForWorkEnrollmentProfile
description: Чтение свойств и связей объекта androidForWorkEnrollmentProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1d518ac3dfacae3c50286d348d141702909ba7d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815714"
---
# <a name="get-androidforworkenrollmentprofile"></a><span data-ttu-id="8226f-103">Получение объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8226f-103">Get androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="8226f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8226f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8226f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8226f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8226f-106">Чтение свойств и связей объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8226f-106">Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8226f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8226f-107">Prerequisites</span></span>
<span data-ttu-id="8226f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8226f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8226f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8226f-110">Permission type</span></span>|<span data-ttu-id="8226f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8226f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8226f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8226f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8226f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8226f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8226f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8226f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8226f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8226f-115">Not supported.</span></span>|
|<span data-ttu-id="8226f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8226f-116">Application</span></span>|<span data-ttu-id="8226f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8226f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8226f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8226f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8226f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8226f-119">Optional query parameters</span></span>
<span data-ttu-id="8226f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8226f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8226f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8226f-121">Request headers</span></span>
|<span data-ttu-id="8226f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8226f-122">Header</span></span>|<span data-ttu-id="8226f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8226f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8226f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8226f-124">Authorization</span></span>|<span data-ttu-id="8226f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8226f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8226f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8226f-126">Accept</span></span>|<span data-ttu-id="8226f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8226f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8226f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8226f-128">Request body</span></span>
<span data-ttu-id="8226f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8226f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8226f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8226f-130">Response</span></span>
<span data-ttu-id="8226f-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8226f-131">If successful, this method returns a `200 OK` response code and [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8226f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8226f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8226f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8226f-133">Request</span></span>
<span data-ttu-id="8226f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8226f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="8226f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8226f-135">Response</span></span>
<span data-ttu-id="8226f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8226f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 719

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
    "accountId": "Account Id value",
    "id": "e6742553-2553-e674-5325-74e6532574e6",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "tokenValue": "Token Value value",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```




