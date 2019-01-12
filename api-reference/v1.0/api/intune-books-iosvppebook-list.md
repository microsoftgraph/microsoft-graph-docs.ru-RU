---
title: Перечисление объектов iosVppEBook
description: Список свойств и связей объектов iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f44d836b3f240b4ac6c59c6b711005a7ab928d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921460"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="6d5c7-103">Перечисление объектов iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="6d5c7-103">List iosVppEBooks</span></span>

> <span data-ttu-id="6d5c7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d5c7-105">Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="6d5c7-105">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d5c7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6d5c7-106">Prerequisites</span></span>
<span data-ttu-id="6d5c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d5c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d5c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d5c7-109">Permission type</span></span>|<span data-ttu-id="6d5c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d5c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d5c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d5c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d5c7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d5c7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d5c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d5c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d5c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-114">Not supported.</span></span>|
|<span data-ttu-id="6d5c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d5c7-115">Application</span></span>|<span data-ttu-id="6d5c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d5c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d5c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="6d5c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d5c7-118">Request headers</span></span>
|<span data-ttu-id="6d5c7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d5c7-119">Header</span></span>|<span data-ttu-id="6d5c7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6d5c7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d5c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d5c7-121">Authorization</span></span>|<span data-ttu-id="6d5c7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d5c7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d5c7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6d5c7-123">Accept</span></span>|<span data-ttu-id="6d5c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d5c7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d5c7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d5c7-125">Request body</span></span>
<span data-ttu-id="6d5c7-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d5c7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d5c7-127">Response</span></span>
<span data-ttu-id="6d5c7-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBook](../resources/intune-books-iosvppebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d5c7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6d5c7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d5c7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d5c7-130">Request</span></span>
<span data-ttu-id="6d5c7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="6d5c7-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d5c7-132">Response</span></span>
<span data-ttu-id="6d5c7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d5c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



