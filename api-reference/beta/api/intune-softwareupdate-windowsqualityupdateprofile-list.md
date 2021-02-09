---
title: Список windowsQualityUpdateProfiles
description: Список свойств и связей объектов windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d124e0db3cb13e529205f5cd939c16920c23b4b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160742"
---
# <a name="list-windowsqualityupdateprofiles"></a><span data-ttu-id="fbb8f-103">Список windowsQualityUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="fbb8f-103">List windowsQualityUpdateProfiles</span></span>

<span data-ttu-id="fbb8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbb8f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbb8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb8f-107">Список свойств и связей объектов [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fbb8f-107">List properties and relationships of the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbb8f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fbb8f-108">Prerequisites</span></span>
<span data-ttu-id="fbb8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbb8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb8f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb8f-111">Permission type</span></span>|<span data-ttu-id="fbb8f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbb8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbb8f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbb8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbb8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbb8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fbb8f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbb8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbb8f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-116">Not supported.</span></span>|
|<span data-ttu-id="fbb8f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbb8f-117">Application</span></span>|<span data-ttu-id="fbb8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbb8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbb8f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbb8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="fbb8f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbb8f-120">Request headers</span></span>
|<span data-ttu-id="fbb8f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbb8f-121">Header</span></span>|<span data-ttu-id="fbb8f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbb8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbb8f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbb8f-123">Authorization</span></span>|<span data-ttu-id="fbb8f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbb8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbb8f-125">Accept</span></span>|<span data-ttu-id="fbb8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbb8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb8f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbb8f-127">Request body</span></span>
<span data-ttu-id="fbb8f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbb8f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb8f-129">Response</span></span>
<span data-ttu-id="fbb8f-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-130">If successful, this method returns a `200 OK` response code and a collection of [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb8f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fbb8f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb8f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbb8f-132">Request</span></span>
<span data-ttu-id="fbb8f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
```

### <a name="response"></a><span data-ttu-id="fbb8f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb8f-134">Response</span></span>
<span data-ttu-id="fbb8f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbb8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
      "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
      "displayName": "Display Name value",
      "description": "Description value",
      "expeditedUpdateSettings": {
        "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
        "qualityUpdateRelease": "Quality Update Release value",
        "daysUntilForcedReboot": 5
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




