---
title: Получение Мобилеаппинсталлсуммари
description: Чтение свойств и связей объекта Мобилеаппинсталлсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11535f724b73d8aa01fcd6ee326878357346bc2c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38079484"
---
# <a name="get-mobileappinstallsummary"></a><span data-ttu-id="3cb0f-103">Получение Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="3cb0f-103">Get mobileAppInstallSummary</span></span>

> <span data-ttu-id="3cb0f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cb0f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb0f-106">Чтение свойств и связей объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3cb0f-106">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cb0f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3cb0f-107">Prerequisites</span></span>
<span data-ttu-id="3cb0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb0f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb0f-110">Permission type</span></span>|<span data-ttu-id="3cb0f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cb0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cb0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb0f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cb0f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3cb0f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cb0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb0f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-115">Not supported.</span></span>|
|<span data-ttu-id="3cb0f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cb0f-116">Application</span></span>|<span data-ttu-id="3cb0f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cb0f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb0f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cb0f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3cb0f-119">Optional query parameters</span></span>
<span data-ttu-id="3cb0f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cb0f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cb0f-121">Request headers</span></span>
|<span data-ttu-id="3cb0f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cb0f-122">Header</span></span>|<span data-ttu-id="3cb0f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3cb0f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cb0f-124">Authorization</span></span>|<span data-ttu-id="3cb0f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cb0f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3cb0f-126">Accept</span></span>|<span data-ttu-id="3cb0f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3cb0f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb0f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cb0f-128">Request body</span></span>
<span data-ttu-id="3cb0f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb0f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cb0f-130">Response</span></span>
<span data-ttu-id="3cb0f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-131">If successful, this method returns a `200 OK` response code and [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cb0f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3cb0f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cb0f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0f-133">Request</span></span>
<span data-ttu-id="3cb0f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

### <a name="response"></a><span data-ttu-id="3cb0f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb0f-135">Response</span></span>
<span data-ttu-id="3cb0f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cb0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






