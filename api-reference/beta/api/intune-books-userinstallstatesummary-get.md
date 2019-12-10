---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82082968afb5c0e60ee46a109f6ca39d10432c4a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930928"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="2c5e3-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="2c5e3-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="2c5e3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c5e3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c5e3-106">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2c5e3-106">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c5e3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2c5e3-107">Prerequisites</span></span>
<span data-ttu-id="2c5e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c5e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c5e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c5e3-110">Permission type</span></span>|<span data-ttu-id="2c5e3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c5e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c5e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c5e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c5e3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c5e3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2c5e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c5e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c5e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-115">Not supported.</span></span>|
|<span data-ttu-id="2c5e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c5e3-116">Application</span></span>|<span data-ttu-id="2c5e3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c5e3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c5e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c5e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c5e3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c5e3-119">Optional query parameters</span></span>
<span data-ttu-id="2c5e3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c5e3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c5e3-121">Request headers</span></span>
|<span data-ttu-id="2c5e3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c5e3-122">Header</span></span>|<span data-ttu-id="2c5e3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2c5e3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c5e3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c5e3-124">Authorization</span></span>|<span data-ttu-id="2c5e3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c5e3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2c5e3-126">Accept</span></span>|<span data-ttu-id="2c5e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c5e3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c5e3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c5e3-128">Request body</span></span>
<span data-ttu-id="2c5e3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c5e3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c5e3-130">Response</span></span>
<span data-ttu-id="2c5e3-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-131">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c5e3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2c5e3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c5e3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c5e3-133">Request</span></span>
<span data-ttu-id="2c5e3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="2c5e3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c5e3-135">Response</span></span>
<span data-ttu-id="2c5e3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c5e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```





