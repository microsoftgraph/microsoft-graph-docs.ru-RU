---
title: Список Виндовсуниверсалаппксконтаинедаппс
description: Список свойств и связей объектов Виндовсуниверсалаппксконтаинедапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57d5d5141c6f9d8ca13808e8e579540b1ee46f9f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693656"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="6f279-103">Список Виндовсуниверсалаппксконтаинедаппс</span><span class="sxs-lookup"><span data-stu-id="6f279-103">List windowsUniversalAppXContainedApps</span></span>

<span data-ttu-id="6f279-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f279-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f279-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f279-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f279-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f279-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f279-107">Список свойств и связей объектов [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6f279-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f279-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f279-108">Prerequisites</span></span>
<span data-ttu-id="6f279-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f279-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f279-111">Permission type</span></span>|<span data-ttu-id="6f279-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f279-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f279-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f279-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f279-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f279-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6f279-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f279-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f279-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f279-116">Not supported.</span></span>|
|<span data-ttu-id="6f279-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f279-117">Application</span></span>|<span data-ttu-id="6f279-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f279-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f279-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f279-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="6f279-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f279-120">Request headers</span></span>
|<span data-ttu-id="6f279-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f279-121">Header</span></span>|<span data-ttu-id="6f279-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f279-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f279-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f279-123">Authorization</span></span>|<span data-ttu-id="6f279-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f279-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f279-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f279-125">Accept</span></span>|<span data-ttu-id="6f279-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f279-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f279-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f279-127">Request body</span></span>
<span data-ttu-id="6f279-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f279-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f279-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f279-129">Response</span></span>
<span data-ttu-id="6f279-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f279-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f279-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6f279-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f279-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f279-132">Request</span></span>
<span data-ttu-id="6f279-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f279-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="6f279-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f279-134">Response</span></span>
<span data-ttu-id="6f279-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f279-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```





