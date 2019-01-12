---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8efef1d8134033cf7e7b96e4fa2b6c047858cc37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918996"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="4eceb-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4eceb-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="4eceb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4eceb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4eceb-105">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4eceb-105">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4eceb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4eceb-106">Prerequisites</span></span>
<span data-ttu-id="4eceb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eceb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eceb-109">Permission type</span></span>|<span data-ttu-id="4eceb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eceb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eceb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eceb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4eceb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eceb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4eceb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eceb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eceb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eceb-114">Not supported.</span></span>|
|<span data-ttu-id="4eceb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eceb-115">Application</span></span>|<span data-ttu-id="4eceb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eceb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eceb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eceb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4eceb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eceb-118">Request headers</span></span>
|<span data-ttu-id="4eceb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eceb-119">Header</span></span>|<span data-ttu-id="4eceb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4eceb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eceb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eceb-121">Authorization</span></span>|<span data-ttu-id="4eceb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4eceb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eceb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4eceb-123">Accept</span></span>|<span data-ttu-id="4eceb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eceb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eceb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4eceb-125">Request body</span></span>
<span data-ttu-id="4eceb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eceb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eceb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eceb-127">Response</span></span>
<span data-ttu-id="4eceb-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eceb-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eceb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4eceb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4eceb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eceb-130">Request</span></span>
<span data-ttu-id="4eceb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eceb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="4eceb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4eceb-132">Response</span></span>
<span data-ttu-id="4eceb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4eceb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



