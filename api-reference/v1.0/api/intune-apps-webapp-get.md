---
title: Get webApp
description: Чтение свойств и связей объекта webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94f056b82d95aa934bc780c957ba174e01b2c4ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580617"
---
# <a name="get-webapp"></a><span data-ttu-id="fb39a-103">Get webApp</span><span class="sxs-lookup"><span data-stu-id="fb39a-103">Get webApp</span></span>

> <span data-ttu-id="fb39a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb39a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb39a-105">Чтение свойств и связей объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb39a-105">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb39a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb39a-106">Prerequisites</span></span>
<span data-ttu-id="fb39a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb39a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb39a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb39a-109">Permission type</span></span>|<span data-ttu-id="fb39a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb39a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb39a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb39a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb39a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb39a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb39a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb39a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb39a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb39a-114">Not supported.</span></span>|
|<span data-ttu-id="fb39a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb39a-115">Application</span></span>|<span data-ttu-id="fb39a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb39a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb39a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb39a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb39a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb39a-118">Optional query parameters</span></span>
<span data-ttu-id="fb39a-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb39a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb39a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb39a-120">Request headers</span></span>
|<span data-ttu-id="fb39a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb39a-121">Header</span></span>|<span data-ttu-id="fb39a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb39a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb39a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb39a-123">Authorization</span></span>|<span data-ttu-id="fb39a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb39a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb39a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb39a-125">Accept</span></span>|<span data-ttu-id="fb39a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb39a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb39a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb39a-127">Request body</span></span>
<span data-ttu-id="fb39a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb39a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb39a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb39a-129">Response</span></span>
<span data-ttu-id="fb39a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb39a-130">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb39a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fb39a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb39a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb39a-132">Request</span></span>
<span data-ttu-id="fb39a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb39a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fb39a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb39a-134">Response</span></span>
<span data-ttu-id="fb39a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb39a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 878

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```



