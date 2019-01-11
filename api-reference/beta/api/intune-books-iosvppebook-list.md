---
title: Перечисление объектов iosVppEBook
description: Список свойств и связей объектов iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5174372e85d808f95ca910b3c57e9c1cc4abc980
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892276"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="4e7b2-103">Перечисление объектов iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="4e7b2-103">List iosVppEBooks</span></span>

> <span data-ttu-id="4e7b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e7b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e7b2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e7b2-107">Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="4e7b2-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e7b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e7b2-108">Prerequisites</span></span>
<span data-ttu-id="4e7b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e7b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e7b2-111">Permission type</span></span>|<span data-ttu-id="4e7b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e7b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e7b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e7b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e7b2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7b2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4e7b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e7b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e7b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-116">Not supported.</span></span>|
|<span data-ttu-id="4e7b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e7b2-117">Application</span></span>|<span data-ttu-id="4e7b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e7b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e7b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="4e7b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e7b2-120">Request headers</span></span>
|<span data-ttu-id="4e7b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e7b2-121">Header</span></span>|<span data-ttu-id="4e7b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e7b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e7b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7b2-123">Authorization</span></span>|<span data-ttu-id="4e7b2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e7b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e7b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e7b2-125">Accept</span></span>|<span data-ttu-id="4e7b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7b2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e7b2-127">Request body</span></span>
<span data-ttu-id="4e7b2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7b2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e7b2-129">Response</span></span>
<span data-ttu-id="4e7b2-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBook](../resources/intune-books-iosvppebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e7b2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4e7b2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e7b2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e7b2-132">Request</span></span>
<span data-ttu-id="4e7b2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="4e7b2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e7b2-134">Response</span></span>
<span data-ttu-id="4e7b2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e7b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





