---
title: Get mobileAppInstallSummary
description: Чтение свойств и связей объекта mobileAppInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a45a94b89c8c40111fcc08fd9127e502ba823d0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139708"
---
# <a name="get-mobileappinstallsummary"></a><span data-ttu-id="2e5ba-103">Get mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2e5ba-103">Get mobileAppInstallSummary</span></span>

<span data-ttu-id="2e5ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e5ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e5ba-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e5ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e5ba-107">Чтение свойств и связей объекта [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ba-107">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e5ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e5ba-108">Prerequisites</span></span>
<span data-ttu-id="2e5ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e5ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5ba-111">Permission type</span></span>|<span data-ttu-id="2e5ba-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e5ba-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e5ba-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e5ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e5ba-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5ba-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e5ba-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e5ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e5ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-116">Not supported.</span></span>|
|<span data-ttu-id="2e5ba-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e5ba-117">Application</span></span>|<span data-ttu-id="2e5ba-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5ba-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e5ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e5ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e5ba-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e5ba-120">Optional query parameters</span></span>
<span data-ttu-id="2e5ba-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e5ba-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e5ba-122">Request headers</span></span>
|<span data-ttu-id="2e5ba-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e5ba-123">Header</span></span>|<span data-ttu-id="2e5ba-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2e5ba-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e5ba-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5ba-125">Authorization</span></span>|<span data-ttu-id="2e5ba-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e5ba-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2e5ba-127">Accept</span></span>|<span data-ttu-id="2e5ba-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e5ba-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e5ba-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e5ba-129">Request body</span></span>
<span data-ttu-id="2e5ba-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e5ba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5ba-131">Response</span></span>
<span data-ttu-id="2e5ba-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-132">If successful, this method returns a `200 OK` response code and [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e5ba-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2e5ba-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e5ba-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e5ba-134">Request</span></span>
<span data-ttu-id="2e5ba-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

### <a name="response"></a><span data-ttu-id="2e5ba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5ba-136">Response</span></span>
<span data-ttu-id="2e5ba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e5ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
    "id": "06a792e9-92e9-06a7-e992-a706e992a706",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notApplicableDeviceCount": 8,
    "notInstalledDeviceCount": 7,
    "pendingInstallDeviceCount": 9,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notApplicableUserCount": 6,
    "notInstalledUserCount": 5,
    "pendingInstallUserCount": 7
  }
}
```




