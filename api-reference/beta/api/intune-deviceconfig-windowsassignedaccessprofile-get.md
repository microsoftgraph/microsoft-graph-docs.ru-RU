---
title: Получение windowsAssignedAccessProfile
description: Чтение свойства и связи объекта windowsAssignedAccessProfile.
author: tfitzmac
ms.openlocfilehash: a4a4fd692c8147283950bb3a2d5de6ebebcd4173
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349765"
---
# <a name="get-windowsassignedaccessprofile"></a><span data-ttu-id="7106d-103">Получение windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="7106d-103">Get windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="7106d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7106d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7106d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7106d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7106d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7106d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7106d-107">Чтение свойства и связи объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7106d-107">Read properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7106d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7106d-108">Prerequisites</span></span>
<span data-ttu-id="7106d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7106d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7106d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7106d-111">Permission type</span></span>|<span data-ttu-id="7106d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7106d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7106d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7106d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7106d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7106d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7106d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7106d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7106d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7106d-116">Not supported.</span></span>|
|<span data-ttu-id="7106d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7106d-117">Application</span></span>|<span data-ttu-id="7106d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7106d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7106d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7106d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7106d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7106d-120">Optional query parameters</span></span>
<span data-ttu-id="7106d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7106d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7106d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7106d-122">Request headers</span></span>
|<span data-ttu-id="7106d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7106d-123">Header</span></span>|<span data-ttu-id="7106d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7106d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7106d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7106d-125">Authorization</span></span>|<span data-ttu-id="7106d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7106d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7106d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7106d-127">Accept</span></span>|<span data-ttu-id="7106d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7106d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7106d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7106d-129">Request body</span></span>
<span data-ttu-id="7106d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7106d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7106d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7106d-131">Response</span></span>
<span data-ttu-id="7106d-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7106d-132">If successful, this method returns a `200 OK` response code and [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7106d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7106d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7106d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7106d-134">Request</span></span>
<span data-ttu-id="7106d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7106d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

### <a name="response"></a><span data-ttu-id="7106d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7106d-136">Response</span></span>
<span data-ttu-id="7106d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7106d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
    "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
    "profileName": "Profile Name value",
    "showTaskBar": true,
    "appUserModelIds": [
      "App User Model Ids value"
    ],
    "desktopAppPaths": [
      "Desktop App Paths value"
    ],
    "userAccounts": [
      "User Accounts value"
    ],
    "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
  }
}
```





