---
title: Список userAppInstallStatuses
description: Свойства списка и связей объектов userAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc9a58c913a62028056484f3b686984d2a9a34f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405550"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="0f635-103">Список userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="0f635-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="0f635-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f635-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f635-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f635-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f635-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f635-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f635-107">Свойства списка и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="0f635-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f635-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0f635-108">Prerequisites</span></span>
<span data-ttu-id="0f635-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f635-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f635-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f635-111">Permission type</span></span>|<span data-ttu-id="0f635-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f635-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f635-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f635-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f635-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f635-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0f635-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f635-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f635-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f635-116">Not supported.</span></span>|
|<span data-ttu-id="0f635-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f635-117">Application</span></span>|<span data-ttu-id="0f635-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f635-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f635-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f635-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0f635-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f635-120">Request headers</span></span>
|<span data-ttu-id="0f635-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f635-121">Header</span></span>|<span data-ttu-id="0f635-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f635-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f635-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f635-123">Authorization</span></span>|<span data-ttu-id="0f635-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0f635-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f635-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f635-125">Accept</span></span>|<span data-ttu-id="0f635-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f635-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f635-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f635-127">Request body</span></span>
<span data-ttu-id="0f635-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f635-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f635-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f635-129">Response</span></span>
<span data-ttu-id="0f635-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0f635-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f635-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0f635-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f635-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f635-132">Request</span></span>
<span data-ttu-id="0f635-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f635-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="0f635-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f635-134">Response</span></span>
<span data-ttu-id="0f635-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0f635-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




