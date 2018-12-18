---
title: Список windowsUniversalAppXContainedApps
description: Свойства списка и связей объектов windowsUniversalAppXContainedApp.
author: tfitzmac
ms.openlocfilehash: f28efa8a32c45d297670789a7726319fd96cc0b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301983"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="a787b-103">Список windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="a787b-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="a787b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a787b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a787b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a787b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a787b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a787b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a787b-107">Свойства списка и связей объектов [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a787b-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a787b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a787b-108">Prerequisites</span></span>
<span data-ttu-id="a787b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a787b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a787b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a787b-111">Permission type</span></span>|<span data-ttu-id="a787b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a787b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a787b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a787b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a787b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a787b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a787b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a787b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a787b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a787b-116">Not supported.</span></span>|
|<span data-ttu-id="a787b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a787b-117">Application</span></span>|<span data-ttu-id="a787b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a787b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a787b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a787b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="a787b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a787b-120">Request headers</span></span>
|<span data-ttu-id="a787b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a787b-121">Header</span></span>|<span data-ttu-id="a787b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a787b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a787b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a787b-123">Authorization</span></span>|<span data-ttu-id="a787b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a787b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a787b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a787b-125">Accept</span></span>|<span data-ttu-id="a787b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a787b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a787b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a787b-127">Request body</span></span>
<span data-ttu-id="a787b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a787b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a787b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a787b-129">Response</span></span>
<span data-ttu-id="a787b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a787b-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a787b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a787b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a787b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a787b-132">Request</span></span>
<span data-ttu-id="a787b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a787b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="a787b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a787b-134">Response</span></span>
<span data-ttu-id="a787b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a787b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





