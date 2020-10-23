---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f3d19b477da0cfddd5191dcca79dc65048e6b83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730271"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="1d38e-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1d38e-103">Get userInstallStateSummary</span></span>

<span data-ttu-id="1d38e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d38e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d38e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d38e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d38e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d38e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d38e-107">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1d38e-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d38e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1d38e-108">Prerequisites</span></span>
<span data-ttu-id="1d38e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d38e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d38e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d38e-111">Permission type</span></span>|<span data-ttu-id="1d38e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d38e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d38e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d38e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d38e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d38e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1d38e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d38e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d38e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d38e-116">Not supported.</span></span>|
|<span data-ttu-id="1d38e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d38e-117">Application</span></span>|<span data-ttu-id="1d38e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d38e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d38e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d38e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d38e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d38e-120">Optional query parameters</span></span>
<span data-ttu-id="1d38e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d38e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d38e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d38e-122">Request headers</span></span>
|<span data-ttu-id="1d38e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d38e-123">Header</span></span>|<span data-ttu-id="1d38e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1d38e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d38e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d38e-125">Authorization</span></span>|<span data-ttu-id="1d38e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d38e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d38e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1d38e-127">Accept</span></span>|<span data-ttu-id="1d38e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d38e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d38e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d38e-129">Request body</span></span>
<span data-ttu-id="1d38e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d38e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d38e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d38e-131">Response</span></span>
<span data-ttu-id="1d38e-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d38e-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d38e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1d38e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d38e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d38e-134">Request</span></span>
<span data-ttu-id="1d38e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d38e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="1d38e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d38e-136">Response</span></span>
<span data-ttu-id="1d38e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d38e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





