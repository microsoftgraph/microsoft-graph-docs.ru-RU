---
title: Get managedMobileLobApp
description: Чтение свойств и связей объекта managedMobileLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06160249d9ca2f2fd4c85a506b4cef6024ae585d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442478"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="e648f-103">Get managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e648f-103">Get managedMobileLobApp</span></span>

<span data-ttu-id="e648f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e648f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e648f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e648f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e648f-106">Чтение свойств и связей объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e648f-106">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e648f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e648f-107">Prerequisites</span></span>
<span data-ttu-id="e648f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e648f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e648f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e648f-110">Permission type</span></span>|<span data-ttu-id="e648f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e648f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e648f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e648f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e648f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e648f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e648f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e648f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e648f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e648f-115">Not supported.</span></span>|
|<span data-ttu-id="e648f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e648f-116">Application</span></span>|<span data-ttu-id="e648f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e648f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e648f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e648f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e648f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e648f-119">Optional query parameters</span></span>
<span data-ttu-id="e648f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e648f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e648f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e648f-121">Request headers</span></span>
|<span data-ttu-id="e648f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e648f-122">Header</span></span>|<span data-ttu-id="e648f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e648f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e648f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e648f-124">Authorization</span></span>|<span data-ttu-id="e648f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e648f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e648f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e648f-126">Accept</span></span>|<span data-ttu-id="e648f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e648f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e648f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e648f-128">Request body</span></span>
<span data-ttu-id="e648f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e648f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e648f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e648f-130">Response</span></span>
<span data-ttu-id="e648f-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e648f-131">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e648f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e648f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e648f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e648f-133">Request</span></span>
<span data-ttu-id="e648f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e648f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e648f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e648f-135">Response</span></span>
<span data-ttu-id="e648f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e648f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```






