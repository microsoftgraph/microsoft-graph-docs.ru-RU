---
title: Получение windowsUniversalAppXContainedApp
description: Чтение свойства и связи объекта windowsUniversalAppXContainedApp.
author: tfitzmac
ms.openlocfilehash: 78d4d015be2e614ddd1d5463824b49281c375d86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311181"
---
# <a name="get-windowsuniversalappxcontainedapp"></a><span data-ttu-id="2effc-103">Получение windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="2effc-103">Get windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="2effc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2effc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2effc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2effc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2effc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2effc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2effc-107">Чтение свойства и связи объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2effc-107">Read properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2effc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2effc-108">Prerequisites</span></span>
<span data-ttu-id="2effc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2effc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2effc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2effc-111">Permission type</span></span>|<span data-ttu-id="2effc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2effc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2effc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2effc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2effc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2effc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2effc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2effc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2effc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2effc-116">Not supported.</span></span>|
|<span data-ttu-id="2effc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2effc-117">Application</span></span>|<span data-ttu-id="2effc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2effc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2effc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2effc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2effc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2effc-120">Optional query parameters</span></span>
<span data-ttu-id="2effc-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2effc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2effc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2effc-122">Request headers</span></span>
|<span data-ttu-id="2effc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2effc-123">Header</span></span>|<span data-ttu-id="2effc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2effc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2effc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2effc-125">Authorization</span></span>|<span data-ttu-id="2effc-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2effc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2effc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2effc-127">Accept</span></span>|<span data-ttu-id="2effc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2effc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2effc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2effc-129">Request body</span></span>
<span data-ttu-id="2effc-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2effc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2effc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2effc-131">Response</span></span>
<span data-ttu-id="2effc-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2effc-132">If successful, this method returns a `200 OK` response code and [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2effc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2effc-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2effc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2effc-134">Request</span></span>
<span data-ttu-id="2effc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2effc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="2effc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2effc-136">Response</span></span>
<span data-ttu-id="2effc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2effc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
    "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
    "appUserModelId": "App User Model Id value"
  }
}
```





