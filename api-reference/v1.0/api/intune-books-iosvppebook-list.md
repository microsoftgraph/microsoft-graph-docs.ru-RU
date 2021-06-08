---
title: Перечисление объектов iosVppEBook
description: Список свойств и связей объектов iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75ab2d3187b6914f6414f03cb5328734e70f7abd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758675"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="690be-103">Перечисление объектов iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="690be-103">List iosVppEBooks</span></span>

<span data-ttu-id="690be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="690be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="690be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="690be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="690be-106">Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="690be-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="690be-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="690be-107">Prerequisites</span></span>
<span data-ttu-id="690be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="690be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="690be-110">Permission type</span></span>|<span data-ttu-id="690be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="690be-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="690be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="690be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="690be-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690be-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="690be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="690be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="690be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="690be-115">Not supported.</span></span>|
|<span data-ttu-id="690be-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="690be-116">Application</span></span>|<span data-ttu-id="690be-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690be-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="690be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="690be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="690be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="690be-119">Request headers</span></span>
|<span data-ttu-id="690be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="690be-120">Header</span></span>|<span data-ttu-id="690be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="690be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="690be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="690be-122">Authorization</span></span>|<span data-ttu-id="690be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="690be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="690be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="690be-124">Accept</span></span>|<span data-ttu-id="690be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="690be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="690be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="690be-126">Request body</span></span>
<span data-ttu-id="690be-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="690be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="690be-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="690be-128">Response</span></span>
<span data-ttu-id="690be-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBook](../resources/intune-books-iosvppebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="690be-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="690be-130">Пример</span><span class="sxs-lookup"><span data-stu-id="690be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="690be-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="690be-131">Request</span></span>
<span data-ttu-id="690be-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="690be-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="690be-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="690be-133">Response</span></span>
<span data-ttu-id="690be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="690be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1097

{
  "value": [
    {
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
      "usedLicenseCount": 0
    }
  ]
}
```




