---
title: Get iosVppEBook
description: Чтение свойств и связей объекта iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb3dd96e037762a8277462e29d03a3e7eb964803
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171297"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="12a3a-103">Get iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="12a3a-103">Get iosVppEBook</span></span>

> <span data-ttu-id="12a3a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a3a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12a3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a3a-106">Чтение свойств и связей объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="12a3a-106">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a3a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="12a3a-107">Prerequisites</span></span>
<span data-ttu-id="12a3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a3a-110">Permission type</span></span>|<span data-ttu-id="12a3a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12a3a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12a3a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12a3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a3a-115">Not supported.</span></span>|
|<span data-ttu-id="12a3a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a3a-116">Application</span></span>|<span data-ttu-id="12a3a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12a3a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12a3a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12a3a-119">Optional query parameters</span></span>
<span data-ttu-id="12a3a-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12a3a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a3a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a3a-121">Request headers</span></span>
|<span data-ttu-id="12a3a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12a3a-122">Header</span></span>|<span data-ttu-id="12a3a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="12a3a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a3a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a3a-124">Authorization</span></span>|<span data-ttu-id="12a3a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a3a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a3a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="12a3a-126">Accept</span></span>|<span data-ttu-id="12a3a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12a3a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a3a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12a3a-128">Request body</span></span>
<span data-ttu-id="12a3a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12a3a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a3a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a3a-130">Response</span></span>
<span data-ttu-id="12a3a-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12a3a-131">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a3a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="12a3a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a3a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a3a-133">Request</span></span>
<span data-ttu-id="12a3a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a3a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="12a3a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a3a-135">Response</span></span>
<span data-ttu-id="12a3a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBook",
    "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
    "largeCover": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "informationUrl": "https://example.com/informationUrl/",
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
    "appleId": "Apple Id value",
    "vppOrganizationName": "Vpp Organization Name value",
    "genres": [
      "Genres value"
    ],
    "language": "Language value",
    "seller": "Seller value",
    "totalLicenseCount": 1,
    "usedLicenseCount": 0,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




