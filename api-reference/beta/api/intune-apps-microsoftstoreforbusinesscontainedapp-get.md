---
title: Получение microsoftStoreForBusinessContainedApp
description: Чтение свойства и связи объекта microsoftStoreForBusinessContainedApp.
author: tfitzmac
ms.openlocfilehash: ee55e0b9ebad6dc42cda2cb2aa996379a6a637c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352243"
---
# <a name="get-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="bd8fd-103">Получение microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="bd8fd-103">Get microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="bd8fd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd8fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd8fd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd8fd-107">Чтение свойства и связи объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bd8fd-107">Read properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd8fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd8fd-108">Prerequisites</span></span>
<span data-ttu-id="bd8fd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd8fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd8fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd8fd-111">Permission type</span></span>|<span data-ttu-id="bd8fd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd8fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd8fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd8fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd8fd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd8fd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd8fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd8fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd8fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-116">Not supported.</span></span>|
|<span data-ttu-id="bd8fd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd8fd-117">Application</span></span>|<span data-ttu-id="bd8fd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd8fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd8fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd8fd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd8fd-120">Optional query parameters</span></span>
<span data-ttu-id="bd8fd-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bd8fd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd8fd-122">Request headers</span></span>
|<span data-ttu-id="bd8fd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd8fd-123">Header</span></span>|<span data-ttu-id="bd8fd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bd8fd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd8fd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd8fd-125">Authorization</span></span>|<span data-ttu-id="bd8fd-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd8fd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd8fd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bd8fd-127">Accept</span></span>|<span data-ttu-id="bd8fd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bd8fd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd8fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd8fd-129">Request body</span></span>
<span data-ttu-id="bd8fd-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd8fd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd8fd-131">Response</span></span>
<span data-ttu-id="bd8fd-132">Успешно завершена, этот метод возвращает `200 OK` объект [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-132">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd8fd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bd8fd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd8fd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd8fd-134">Request</span></span>
<span data-ttu-id="bd8fd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="bd8fd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd8fd-136">Response</span></span>
<span data-ttu-id="bd8fd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd8fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
    "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
    "appUserModelId": "App User Model Id value"
  }
}
```





