---
title: Получение userAppInstallStatus
description: Чтение свойства и связи объекта userAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 800afbf864d9e56b3ef3d010e50ebb99a5e8ecf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864549"
---
# <a name="get-userappinstallstatus"></a><span data-ttu-id="019df-103">Получение userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="019df-103">Get userAppInstallStatus</span></span>

> <span data-ttu-id="019df-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="019df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="019df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="019df-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="019df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="019df-107">Чтение свойства и связи объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="019df-107">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="019df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="019df-108">Prerequisites</span></span>
<span data-ttu-id="019df-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="019df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="019df-111">Permission type</span></span>|<span data-ttu-id="019df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="019df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="019df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="019df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="019df-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="019df-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="019df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="019df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="019df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019df-116">Not supported.</span></span>|
|<span data-ttu-id="019df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="019df-117">Application</span></span>|<span data-ttu-id="019df-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="019df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="019df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="019df-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="019df-120">Optional query parameters</span></span>
<span data-ttu-id="019df-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="019df-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="019df-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="019df-122">Request headers</span></span>
|<span data-ttu-id="019df-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="019df-123">Header</span></span>|<span data-ttu-id="019df-124">Значение</span><span class="sxs-lookup"><span data-stu-id="019df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="019df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="019df-125">Authorization</span></span>|<span data-ttu-id="019df-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="019df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="019df-127">Accept</span><span class="sxs-lookup"><span data-stu-id="019df-127">Accept</span></span>|<span data-ttu-id="019df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="019df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="019df-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="019df-129">Request body</span></span>
<span data-ttu-id="019df-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="019df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="019df-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="019df-131">Response</span></span>
<span data-ttu-id="019df-132">Успешно завершена, этот метод возвращает `200 OK` объект [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="019df-132">If successful, this method returns a `200 OK` response code and [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="019df-133">Пример</span><span class="sxs-lookup"><span data-stu-id="019df-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="019df-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="019df-134">Request</span></span>
<span data-ttu-id="019df-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="019df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="019df-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="019df-136">Response</span></span>
<span data-ttu-id="019df-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="019df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "value": {
    "@odata.type": "#microsoft.graph.userAppInstallStatus",
    "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```





