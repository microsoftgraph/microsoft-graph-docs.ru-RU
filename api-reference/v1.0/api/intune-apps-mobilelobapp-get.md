---
title: Get mobileLobApp
description: Чтение свойств и связей объекта mobileLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 923da86cef63e39ca603494d2ae3e3192f1566d7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250154"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="a5949-103">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="a5949-103">Get mobileLobApp</span></span>

> <span data-ttu-id="a5949-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5949-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5949-105">Чтение свойств и связей объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a5949-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5949-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a5949-106">Prerequisites</span></span>
<span data-ttu-id="a5949-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5949-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5949-109">Permission type</span></span>|<span data-ttu-id="a5949-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5949-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5949-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5949-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5949-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5949-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a5949-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5949-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5949-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5949-114">Not supported.</span></span>|
|<span data-ttu-id="a5949-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5949-115">Application</span></span>|<span data-ttu-id="a5949-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5949-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5949-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5949-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5949-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5949-118">Optional query parameters</span></span>
<span data-ttu-id="a5949-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5949-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5949-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5949-120">Request headers</span></span>
|<span data-ttu-id="a5949-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5949-121">Header</span></span>|<span data-ttu-id="a5949-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5949-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5949-123">Authorization</span></span>|<span data-ttu-id="a5949-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a5949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5949-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5949-125">Accept</span></span>|<span data-ttu-id="a5949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5949-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5949-127">Request body</span></span>
<span data-ttu-id="a5949-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5949-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5949-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5949-129">Response</span></span>
<span data-ttu-id="a5949-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileLobApp](../resources/intune-apps-mobilelobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a5949-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5949-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a5949-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5949-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5949-132">Request</span></span>
<span data-ttu-id="a5949-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5949-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a5949-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5949-134">Response</span></span>
<span data-ttu-id="a5949-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a5949-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



