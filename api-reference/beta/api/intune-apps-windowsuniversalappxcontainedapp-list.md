---
title: Список windowsUniversalAppXContainedApps
description: Свойства списка и связей объектов windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f5c7afb65c3628629d5349bca76c1b46467dfc9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808689"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="22baf-103">Список windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="22baf-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="22baf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22baf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22baf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22baf-107">Свойства списка и связей объектов [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="22baf-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22baf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22baf-108">Prerequisites</span></span>
<span data-ttu-id="22baf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22baf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22baf-111">Permission type</span></span>|<span data-ttu-id="22baf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22baf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22baf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="22baf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="22baf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22baf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22baf-116">Not supported.</span></span>|
|<span data-ttu-id="22baf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22baf-117">Application</span></span>|<span data-ttu-id="22baf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22baf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="22baf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22baf-120">Request headers</span></span>
|<span data-ttu-id="22baf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22baf-121">Header</span></span>|<span data-ttu-id="22baf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22baf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22baf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22baf-123">Authorization</span></span>|<span data-ttu-id="22baf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22baf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22baf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22baf-125">Accept</span></span>|<span data-ttu-id="22baf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22baf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22baf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22baf-127">Request body</span></span>
<span data-ttu-id="22baf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22baf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22baf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="22baf-129">Response</span></span>
<span data-ttu-id="22baf-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22baf-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22baf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="22baf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="22baf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="22baf-132">Request</span></span>
<span data-ttu-id="22baf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22baf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="22baf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="22baf-134">Response</span></span>
<span data-ttu-id="22baf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="22baf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





