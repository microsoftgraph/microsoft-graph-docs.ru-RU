---
title: Список mobileAppProvisioningConfigGroupAssignments
description: Свойства списка и связей объектов mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b582847ca8862ccb00150ec6d8b6bbf850b3d1e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925828"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="c1573-103">Список mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="c1573-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="c1573-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1573-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1573-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1573-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1573-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1573-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1573-107">Свойства списка и связей объектов [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c1573-107">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1573-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1573-108">Prerequisites</span></span>
<span data-ttu-id="c1573-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1573-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1573-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1573-111">Permission type</span></span>|<span data-ttu-id="c1573-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1573-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1573-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1573-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1573-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1573-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1573-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1573-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1573-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1573-116">Not supported.</span></span>|
|<span data-ttu-id="c1573-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1573-117">Application</span></span>|<span data-ttu-id="c1573-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1573-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1573-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1573-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c1573-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1573-120">Request headers</span></span>
|<span data-ttu-id="c1573-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1573-121">Header</span></span>|<span data-ttu-id="c1573-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1573-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1573-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1573-123">Authorization</span></span>|<span data-ttu-id="c1573-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c1573-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1573-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1573-125">Accept</span></span>|<span data-ttu-id="c1573-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1573-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1573-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1573-127">Request body</span></span>
<span data-ttu-id="c1573-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1573-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1573-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1573-129">Response</span></span>
<span data-ttu-id="c1573-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1573-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1573-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c1573-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1573-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1573-132">Request</span></span>
<span data-ttu-id="c1573-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1573-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="c1573-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1573-134">Response</span></span>
<span data-ttu-id="c1573-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c1573-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```





