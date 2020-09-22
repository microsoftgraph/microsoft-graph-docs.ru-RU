---
title: Get managedEBook
description: Чтение свойств и связей объекта managedEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ee0ecc9f3dd0bbc52319beca03e95e5727ed6b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077886"
---
# <a name="get-managedebook"></a><span data-ttu-id="92103-103">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="92103-103">Get managedEBook</span></span>

<span data-ttu-id="92103-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92103-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92103-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92103-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92103-106">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="92103-106">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92103-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="92103-107">Prerequisites</span></span>
<span data-ttu-id="92103-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92103-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92103-110">Permission type</span></span>|<span data-ttu-id="92103-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92103-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92103-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92103-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92103-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92103-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92103-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92103-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92103-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92103-115">Not supported.</span></span>|
|<span data-ttu-id="92103-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92103-116">Application</span></span>|<span data-ttu-id="92103-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92103-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92103-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92103-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92103-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92103-119">Optional query parameters</span></span>
<span data-ttu-id="92103-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92103-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92103-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92103-121">Request headers</span></span>
|<span data-ttu-id="92103-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92103-122">Header</span></span>|<span data-ttu-id="92103-123">Значение</span><span class="sxs-lookup"><span data-stu-id="92103-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92103-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92103-124">Authorization</span></span>|<span data-ttu-id="92103-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92103-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92103-126">Accept</span><span class="sxs-lookup"><span data-stu-id="92103-126">Accept</span></span>|<span data-ttu-id="92103-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92103-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92103-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92103-128">Request body</span></span>
<span data-ttu-id="92103-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92103-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92103-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="92103-130">Response</span></span>
<span data-ttu-id="92103-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBook](../resources/intune-books-managedebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="92103-131">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92103-132">Пример</span><span class="sxs-lookup"><span data-stu-id="92103-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="92103-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="92103-133">Request</span></span>
<span data-ttu-id="92103-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92103-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="92103-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="92103-135">Response</span></span>
<span data-ttu-id="92103-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92103-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









