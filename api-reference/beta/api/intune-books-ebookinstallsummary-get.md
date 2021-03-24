---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc20853eda7a1a3785dcbf6e40f871b2ea5ddd93
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133684"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="15b82-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="15b82-103">Get eBookInstallSummary</span></span>

<span data-ttu-id="15b82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15b82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15b82-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15b82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15b82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15b82-107">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="15b82-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15b82-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="15b82-108">Prerequisites</span></span>
<span data-ttu-id="15b82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15b82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15b82-111">Permission type</span></span>|<span data-ttu-id="15b82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15b82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15b82-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15b82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15b82-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b82-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15b82-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15b82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15b82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b82-116">Not supported.</span></span>|
|<span data-ttu-id="15b82-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="15b82-117">Application</span></span>|<span data-ttu-id="15b82-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b82-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15b82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15b82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15b82-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15b82-120">Optional query parameters</span></span>
<span data-ttu-id="15b82-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15b82-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15b82-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15b82-122">Request headers</span></span>
|<span data-ttu-id="15b82-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15b82-123">Header</span></span>|<span data-ttu-id="15b82-124">Значение</span><span class="sxs-lookup"><span data-stu-id="15b82-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15b82-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="15b82-125">Authorization</span></span>|<span data-ttu-id="15b82-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15b82-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15b82-127">Accept</span><span class="sxs-lookup"><span data-stu-id="15b82-127">Accept</span></span>|<span data-ttu-id="15b82-128">application/json</span><span class="sxs-lookup"><span data-stu-id="15b82-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15b82-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15b82-129">Request body</span></span>
<span data-ttu-id="15b82-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15b82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15b82-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b82-131">Response</span></span>
<span data-ttu-id="15b82-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15b82-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15b82-133">Пример</span><span class="sxs-lookup"><span data-stu-id="15b82-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="15b82-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="15b82-134">Request</span></span>
<span data-ttu-id="15b82-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15b82-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="15b82-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b82-136">Response</span></span>
<span data-ttu-id="15b82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15b82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




