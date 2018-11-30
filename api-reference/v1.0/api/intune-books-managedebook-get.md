---
title: Get managedEBook
description: Чтение свойств и связей объекта managedEBook.
ms.openlocfilehash: 852bce05d023dc2adff92ccb670da2b9996d45af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024990"
---
# <a name="get-managedebook"></a><span data-ttu-id="aaf87-103">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="aaf87-103">Get managedEBook</span></span>

> <span data-ttu-id="aaf87-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aaf87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaf87-105">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="aaf87-105">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaf87-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf87-106">Prerequisites</span></span>
<span data-ttu-id="aaf87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf87-109">Permission type</span></span>|<span data-ttu-id="aaf87-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaf87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaf87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaf87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aaf87-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaf87-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aaf87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaf87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaf87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaf87-114">Not supported.</span></span>|
|<span data-ttu-id="aaf87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaf87-115">Application</span></span>|<span data-ttu-id="aaf87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaf87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaf87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaf87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaf87-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aaf87-118">Optional query parameters</span></span>
<span data-ttu-id="aaf87-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aaf87-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aaf87-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaf87-120">Request headers</span></span>
|<span data-ttu-id="aaf87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aaf87-121">Header</span></span>|<span data-ttu-id="aaf87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aaf87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaf87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf87-123">Authorization</span></span>|<span data-ttu-id="aaf87-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aaf87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaf87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aaf87-125">Accept</span></span>|<span data-ttu-id="aaf87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaf87-127">Request body</span></span>
<span data-ttu-id="aaf87-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaf87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaf87-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aaf87-129">Response</span></span>
<span data-ttu-id="aaf87-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBook](../resources/intune-books-managedebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aaf87-130">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf87-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aaf87-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaf87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaf87-132">Request</span></span>
<span data-ttu-id="aaf87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaf87-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="aaf87-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="aaf87-134">Response</span></span>
<span data-ttu-id="aaf87-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="aaf87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBook",
    "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
  }
}
```



