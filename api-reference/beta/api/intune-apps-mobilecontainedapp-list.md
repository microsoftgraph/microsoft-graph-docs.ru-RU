---
title: Список mobileContainedApps
description: Свойства списка и связей объектов mobileContainedApp.
ms.openlocfilehash: 77f15813f2f6a7b15d365e93d48bd3c923d36354
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077231"
---
# <a name="list-mobilecontainedapps"></a><span data-ttu-id="52f4a-103">Список mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="52f4a-103">List mobileContainedApps</span></span>

> <span data-ttu-id="52f4a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52f4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52f4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52f4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52f4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52f4a-107">Свойства списка и связей объектов [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="52f4a-107">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52f4a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52f4a-108">Prerequisites</span></span>
<span data-ttu-id="52f4a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52f4a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f4a-111">Permission type</span></span>|<span data-ttu-id="52f4a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52f4a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52f4a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="52f4a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="52f4a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f4a-116">Not supported.</span></span>|
|<span data-ttu-id="52f4a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52f4a-117">Application</span></span>|<span data-ttu-id="52f4a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f4a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="52f4a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f4a-120">Request headers</span></span>
|<span data-ttu-id="52f4a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52f4a-121">Header</span></span>|<span data-ttu-id="52f4a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52f4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52f4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52f4a-123">Authorization</span></span>|<span data-ttu-id="52f4a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="52f4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52f4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52f4a-125">Accept</span></span>|<span data-ttu-id="52f4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52f4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f4a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f4a-127">Request body</span></span>
<span data-ttu-id="52f4a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52f4a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52f4a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f4a-129">Response</span></span>
<span data-ttu-id="52f4a-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52f4a-130">If successful, this method returns a `200 OK` response code and a collection of [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f4a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="52f4a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="52f4a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f4a-132">Request</span></span>
<span data-ttu-id="52f4a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52f4a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="52f4a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f4a-134">Response</span></span>
<span data-ttu-id="52f4a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="52f4a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 150

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileContainedApp",
      "id": "3c02d875-d875-3c02-75d8-023c75d8023c"
    }
  ]
}
```





