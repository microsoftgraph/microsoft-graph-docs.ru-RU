---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bdef80ffc31450adb175e310e56b3ae5e629f1f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423230"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="a38fa-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a38fa-103">Get eBookInstallSummary</span></span>

<span data-ttu-id="a38fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a38fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a38fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a38fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a38fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a38fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a38fa-107">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a38fa-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a38fa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a38fa-108">Prerequisites</span></span>
<span data-ttu-id="a38fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a38fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a38fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a38fa-111">Permission type</span></span>|<span data-ttu-id="a38fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a38fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a38fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a38fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a38fa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a38fa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a38fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a38fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a38fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a38fa-116">Not supported.</span></span>|
|<span data-ttu-id="a38fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a38fa-117">Application</span></span>|<span data-ttu-id="a38fa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a38fa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a38fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a38fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a38fa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a38fa-120">Optional query parameters</span></span>
<span data-ttu-id="a38fa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a38fa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a38fa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a38fa-122">Request headers</span></span>
|<span data-ttu-id="a38fa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a38fa-123">Header</span></span>|<span data-ttu-id="a38fa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a38fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a38fa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a38fa-125">Authorization</span></span>|<span data-ttu-id="a38fa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a38fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a38fa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a38fa-127">Accept</span></span>|<span data-ttu-id="a38fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a38fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a38fa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a38fa-129">Request body</span></span>
<span data-ttu-id="a38fa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a38fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a38fa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a38fa-131">Response</span></span>
<span data-ttu-id="a38fa-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a38fa-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a38fa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a38fa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a38fa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a38fa-134">Request</span></span>
<span data-ttu-id="a38fa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a38fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="a38fa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a38fa-136">Response</span></span>
<span data-ttu-id="a38fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a38fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



