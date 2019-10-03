---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2dff8df3346edf0fabfe489998964159244b843e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368444"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="8a6be-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8a6be-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="8a6be-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a6be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a6be-105">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8a6be-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a6be-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8a6be-106">Prerequisites</span></span>
<span data-ttu-id="8a6be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a6be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a6be-109">Permission type</span></span>|<span data-ttu-id="8a6be-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a6be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a6be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a6be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a6be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a6be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a6be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a6be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a6be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a6be-114">Not supported.</span></span>|
|<span data-ttu-id="8a6be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a6be-115">Application</span></span>|<span data-ttu-id="8a6be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a6be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a6be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a6be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a6be-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8a6be-118">Optional query parameters</span></span>
<span data-ttu-id="8a6be-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8a6be-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a6be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a6be-120">Request headers</span></span>
|<span data-ttu-id="8a6be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a6be-121">Header</span></span>|<span data-ttu-id="8a6be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a6be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a6be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a6be-123">Authorization</span></span>|<span data-ttu-id="8a6be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a6be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a6be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a6be-125">Accept</span></span>|<span data-ttu-id="8a6be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a6be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a6be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a6be-127">Request body</span></span>
<span data-ttu-id="8a6be-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a6be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a6be-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a6be-129">Response</span></span>
<span data-ttu-id="8a6be-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8a6be-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a6be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8a6be-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a6be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a6be-132">Request</span></span>
<span data-ttu-id="8a6be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a6be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8a6be-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a6be-134">Response</span></span>
<span data-ttu-id="8a6be-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a6be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




