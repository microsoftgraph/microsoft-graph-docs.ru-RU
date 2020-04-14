---
title: Список Усераппинсталлстатусес
description: Список свойств и связей объектов Усераппинсталлстатус.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4eb2ddabef08a0819fee7ae49ec61150958c8e0b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403845"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="6a84d-103">Список Усераппинсталлстатусес</span><span class="sxs-lookup"><span data-stu-id="6a84d-103">List userAppInstallStatuses</span></span>

<span data-ttu-id="6a84d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a84d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a84d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a84d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a84d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a84d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a84d-107">Список свойств и связей объектов [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6a84d-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a84d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a84d-108">Prerequisites</span></span>
<span data-ttu-id="6a84d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a84d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a84d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a84d-111">Permission type</span></span>|<span data-ttu-id="6a84d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a84d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a84d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a84d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a84d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a84d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a84d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a84d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a84d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a84d-116">Not supported.</span></span>|
|<span data-ttu-id="6a84d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6a84d-117">Application</span></span>|<span data-ttu-id="6a84d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a84d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a84d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a84d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6a84d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a84d-120">Request headers</span></span>
|<span data-ttu-id="6a84d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a84d-121">Header</span></span>|<span data-ttu-id="6a84d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a84d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a84d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a84d-123">Authorization</span></span>|<span data-ttu-id="6a84d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a84d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a84d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a84d-125">Accept</span></span>|<span data-ttu-id="6a84d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a84d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a84d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a84d-127">Request body</span></span>
<span data-ttu-id="6a84d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a84d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a84d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a84d-129">Response</span></span>
<span data-ttu-id="6a84d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a84d-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a84d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6a84d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a84d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a84d-132">Request</span></span>
<span data-ttu-id="6a84d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a84d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="6a84d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a84d-134">Response</span></span>
<span data-ttu-id="6a84d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a84d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```



