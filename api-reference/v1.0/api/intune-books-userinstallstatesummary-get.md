---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8e33f71e5a4b7008e7dc2b46fab5c04023ce579
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972629"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="172bc-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="172bc-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="172bc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="172bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="172bc-105">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="172bc-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="172bc-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="172bc-106">Prerequisites</span></span>
<span data-ttu-id="172bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="172bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="172bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="172bc-109">Permission type</span></span>|<span data-ttu-id="172bc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="172bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="172bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="172bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="172bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="172bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="172bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="172bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="172bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="172bc-114">Not supported.</span></span>|
|<span data-ttu-id="172bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="172bc-115">Application</span></span>|<span data-ttu-id="172bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="172bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="172bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="172bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="172bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="172bc-118">Optional query parameters</span></span>
<span data-ttu-id="172bc-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="172bc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="172bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="172bc-120">Request headers</span></span>
|<span data-ttu-id="172bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="172bc-121">Header</span></span>|<span data-ttu-id="172bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="172bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="172bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="172bc-123">Authorization</span></span>|<span data-ttu-id="172bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="172bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="172bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="172bc-125">Accept</span></span>|<span data-ttu-id="172bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="172bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="172bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="172bc-127">Request body</span></span>
<span data-ttu-id="172bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="172bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="172bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="172bc-129">Response</span></span>
<span data-ttu-id="172bc-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="172bc-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="172bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="172bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="172bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="172bc-132">Request</span></span>
<span data-ttu-id="172bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="172bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="172bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="172bc-134">Response</span></span>
<span data-ttu-id="172bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="172bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



