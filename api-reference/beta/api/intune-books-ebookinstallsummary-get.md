---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 274e357929770be52e4ea233f7c84e76f58ac4fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450372"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="4f703-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="4f703-103">Get eBookInstallSummary</span></span>

<span data-ttu-id="4f703-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f703-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f703-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f703-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f703-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f703-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f703-107">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4f703-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f703-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f703-108">Prerequisites</span></span>
<span data-ttu-id="4f703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f703-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f703-111">Permission type</span></span>|<span data-ttu-id="4f703-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f703-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f703-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f703-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f703-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f703-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4f703-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f703-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f703-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f703-116">Not supported.</span></span>|
|<span data-ttu-id="4f703-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f703-117">Application</span></span>|<span data-ttu-id="4f703-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f703-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f703-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f703-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f703-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f703-120">Optional query parameters</span></span>
<span data-ttu-id="4f703-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f703-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f703-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f703-122">Request headers</span></span>
|<span data-ttu-id="4f703-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f703-123">Header</span></span>|<span data-ttu-id="4f703-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f703-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f703-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f703-125">Authorization</span></span>|<span data-ttu-id="4f703-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f703-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f703-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f703-127">Accept</span></span>|<span data-ttu-id="4f703-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f703-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f703-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f703-129">Request body</span></span>
<span data-ttu-id="4f703-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f703-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f703-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f703-131">Response</span></span>
<span data-ttu-id="4f703-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f703-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f703-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4f703-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f703-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f703-134">Request</span></span>
<span data-ttu-id="4f703-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f703-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="4f703-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f703-136">Response</span></span>
<span data-ttu-id="4f703-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f703-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





