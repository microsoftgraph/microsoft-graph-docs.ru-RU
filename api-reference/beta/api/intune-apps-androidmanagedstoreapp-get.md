---
title: Получение androidManagedStoreApp
description: Чтение свойства и связи объекта androidManagedStoreApp.
author: tfitzmac
ms.openlocfilehash: 8c284d12ef98105e5e241913c9505c0645bb8968
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360174"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="be92f-103">Получение androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="be92f-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="be92f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be92f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be92f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be92f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be92f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be92f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be92f-107">Чтение свойства и связи объекта [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="be92f-107">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be92f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be92f-108">Prerequisites</span></span>
<span data-ttu-id="be92f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be92f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be92f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be92f-111">Permission type</span></span>|<span data-ttu-id="be92f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be92f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be92f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be92f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be92f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="be92f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="be92f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be92f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be92f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be92f-116">Not supported.</span></span>|
|<span data-ttu-id="be92f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be92f-117">Application</span></span>|<span data-ttu-id="be92f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be92f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be92f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be92f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be92f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be92f-120">Optional query parameters</span></span>
<span data-ttu-id="be92f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be92f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be92f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be92f-122">Request headers</span></span>
|<span data-ttu-id="be92f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be92f-123">Header</span></span>|<span data-ttu-id="be92f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="be92f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be92f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be92f-125">Authorization</span></span>|<span data-ttu-id="be92f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be92f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be92f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="be92f-127">Accept</span></span>|<span data-ttu-id="be92f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be92f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be92f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be92f-129">Request body</span></span>
<span data-ttu-id="be92f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be92f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be92f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="be92f-131">Response</span></span>
<span data-ttu-id="be92f-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be92f-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be92f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="be92f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="be92f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="be92f-134">Request</span></span>
<span data-ttu-id="be92f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be92f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="be92f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="be92f-136">Response</span></span>
<span data-ttu-id="be92f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be92f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1037

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreApp",
    "id": "87247525-7525-8724-2575-248725752487",
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
    "uploadState": 11,
    "publishingState": "processing",
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```





