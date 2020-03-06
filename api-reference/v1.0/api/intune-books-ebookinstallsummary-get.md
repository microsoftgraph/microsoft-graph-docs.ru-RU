---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1d7774c445cb43d2b089f117442c8b0745508b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515688"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="e6d59-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e6d59-103">Get eBookInstallSummary</span></span>

<span data-ttu-id="e6d59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6d59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6d59-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6d59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6d59-106">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e6d59-106">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6d59-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d59-107">Prerequisites</span></span>
<span data-ttu-id="e6d59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6d59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d59-110">Permission type</span></span>|<span data-ttu-id="e6d59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6d59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6d59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6d59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6d59-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6d59-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e6d59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6d59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6d59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6d59-115">Not supported.</span></span>|
|<span data-ttu-id="e6d59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6d59-116">Application</span></span>|<span data-ttu-id="e6d59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6d59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6d59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6d59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6d59-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6d59-119">Optional query parameters</span></span>
<span data-ttu-id="e6d59-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6d59-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6d59-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6d59-121">Request headers</span></span>
|<span data-ttu-id="e6d59-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6d59-122">Header</span></span>|<span data-ttu-id="e6d59-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e6d59-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6d59-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6d59-124">Authorization</span></span>|<span data-ttu-id="e6d59-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6d59-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6d59-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e6d59-126">Accept</span></span>|<span data-ttu-id="e6d59-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e6d59-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6d59-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6d59-128">Request body</span></span>
<span data-ttu-id="e6d59-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6d59-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6d59-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6d59-130">Response</span></span>
<span data-ttu-id="e6d59-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6d59-131">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6d59-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e6d59-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6d59-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6d59-133">Request</span></span>
<span data-ttu-id="e6d59-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6d59-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="e6d59-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6d59-135">Response</span></span>
<span data-ttu-id="e6d59-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6d59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```




