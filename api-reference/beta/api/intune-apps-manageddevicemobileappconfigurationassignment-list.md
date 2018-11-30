---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
ms.openlocfilehash: c189801537f0ae191e138edca95080c0cb6d55d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077490"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="9e3cf-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9e3cf-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="9e3cf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e3cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e3cf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e3cf-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9e3cf-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e3cf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9e3cf-108">Prerequisites</span></span>
<span data-ttu-id="9e3cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e3cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e3cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e3cf-111">Permission type</span></span>|<span data-ttu-id="9e3cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e3cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e3cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e3cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e3cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e3cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9e3cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e3cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e3cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-116">Not supported.</span></span>|
|<span data-ttu-id="9e3cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e3cf-117">Application</span></span>|<span data-ttu-id="9e3cf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e3cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e3cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9e3cf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e3cf-120">Request headers</span></span>
|<span data-ttu-id="9e3cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e3cf-121">Header</span></span>|<span data-ttu-id="9e3cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9e3cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e3cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e3cf-123">Authorization</span></span>|<span data-ttu-id="9e3cf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9e3cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e3cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e3cf-125">Accept</span></span>|<span data-ttu-id="9e3cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e3cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e3cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e3cf-127">Request body</span></span>
<span data-ttu-id="9e3cf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e3cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e3cf-129">Response</span></span>
<span data-ttu-id="9e3cf-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e3cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e3cf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e3cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e3cf-132">Request</span></span>
<span data-ttu-id="9e3cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="9e3cf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e3cf-134">Response</span></span>
<span data-ttu-id="9e3cf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9e3cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





