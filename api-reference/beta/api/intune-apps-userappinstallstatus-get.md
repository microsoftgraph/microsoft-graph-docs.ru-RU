---
title: Получение Усераппинсталлстатус
description: Чтение свойств и связей объекта Усераппинсталлстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6192d15665ddb48d8afe3a6d28d98e642d3ac4c8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172228"
---
# <a name="get-userappinstallstatus"></a><span data-ttu-id="3dd69-103">Получение Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="3dd69-103">Get userAppInstallStatus</span></span>

> <span data-ttu-id="3dd69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dd69-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3dd69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dd69-106">Чтение свойств и связей объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="3dd69-106">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dd69-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3dd69-107">Prerequisites</span></span>
<span data-ttu-id="3dd69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dd69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd69-110">Permission type</span></span>|<span data-ttu-id="3dd69-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dd69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dd69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dd69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3dd69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dd69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3dd69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dd69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dd69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd69-115">Not supported.</span></span>|
|<span data-ttu-id="3dd69-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dd69-116">Application</span></span>|<span data-ttu-id="3dd69-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dd69-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dd69-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dd69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dd69-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3dd69-119">Optional query parameters</span></span>
<span data-ttu-id="3dd69-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3dd69-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dd69-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3dd69-121">Request headers</span></span>
|<span data-ttu-id="3dd69-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3dd69-122">Header</span></span>|<span data-ttu-id="3dd69-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3dd69-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dd69-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3dd69-124">Authorization</span></span>|<span data-ttu-id="3dd69-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd69-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dd69-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3dd69-126">Accept</span></span>|<span data-ttu-id="3dd69-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3dd69-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dd69-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3dd69-128">Request body</span></span>
<span data-ttu-id="3dd69-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3dd69-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dd69-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3dd69-130">Response</span></span>
<span data-ttu-id="3dd69-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3dd69-131">If successful, this method returns a `200 OK` response code and [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd69-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3dd69-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dd69-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dd69-133">Request</span></span>
<span data-ttu-id="3dd69-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dd69-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="3dd69-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dd69-135">Response</span></span>
<span data-ttu-id="3dd69-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3dd69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




