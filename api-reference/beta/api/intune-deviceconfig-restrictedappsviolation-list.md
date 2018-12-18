---
title: Список restrictedAppsViolations
description: Свойства списка и связей объектов restrictedAppsViolation.
author: tfitzmac
ms.openlocfilehash: 7c39927b681953296bb23715457a7353151e58b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327820"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="db2ed-103">Список restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="db2ed-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="db2ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db2ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db2ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db2ed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="db2ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db2ed-107">Свойства списка и связей объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="db2ed-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db2ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db2ed-108">Prerequisites</span></span>
<span data-ttu-id="db2ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db2ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db2ed-111">Permission type</span></span>|<span data-ttu-id="db2ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db2ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db2ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db2ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db2ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db2ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db2ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db2ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db2ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2ed-116">Not supported.</span></span>|
|<span data-ttu-id="db2ed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db2ed-117">Application</span></span>|<span data-ttu-id="db2ed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db2ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db2ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="db2ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db2ed-120">Request headers</span></span>
|<span data-ttu-id="db2ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db2ed-121">Header</span></span>|<span data-ttu-id="db2ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db2ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db2ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db2ed-123">Authorization</span></span>|<span data-ttu-id="db2ed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="db2ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db2ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db2ed-125">Accept</span></span>|<span data-ttu-id="db2ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db2ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db2ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db2ed-127">Request body</span></span>
<span data-ttu-id="db2ed-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db2ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db2ed-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="db2ed-129">Response</span></span>
<span data-ttu-id="db2ed-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db2ed-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db2ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="db2ed-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="db2ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db2ed-132">Request</span></span>
<span data-ttu-id="db2ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db2ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="db2ed-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="db2ed-134">Response</span></span>
<span data-ttu-id="db2ed-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="db2ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





