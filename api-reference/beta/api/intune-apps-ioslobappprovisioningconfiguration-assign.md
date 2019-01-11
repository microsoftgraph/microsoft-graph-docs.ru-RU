---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7b7f92592a0ece8169b4f4148e71df5b6297ca7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824412"
---
# <a name="assign-action"></a><span data-ttu-id="e5498-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e5498-103">assign action</span></span>

> <span data-ttu-id="e5498-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5498-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5498-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5498-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5498-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5498-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5498-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5498-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5498-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5498-108">Prerequisites</span></span>
<span data-ttu-id="e5498-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5498-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5498-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5498-111">Permission type</span></span>|<span data-ttu-id="e5498-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5498-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5498-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5498-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5498-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5498-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5498-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5498-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5498-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5498-116">Not supported.</span></span>|
|<span data-ttu-id="e5498-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5498-117">Application</span></span>|<span data-ttu-id="e5498-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5498-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5498-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5498-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e5498-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5498-120">Request headers</span></span>
|<span data-ttu-id="e5498-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5498-121">Header</span></span>|<span data-ttu-id="e5498-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5498-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5498-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5498-123">Authorization</span></span>|<span data-ttu-id="e5498-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e5498-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5498-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5498-125">Accept</span></span>|<span data-ttu-id="e5498-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5498-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5498-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5498-127">Request body</span></span>
<span data-ttu-id="e5498-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5498-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e5498-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e5498-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e5498-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5498-130">Property</span></span>|<span data-ttu-id="e5498-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5498-131">Type</span></span>|<span data-ttu-id="e5498-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5498-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5498-133">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="e5498-133">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="e5498-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e5498-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="e5498-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5498-135">Not yet documented</span></span>|
|<span data-ttu-id="e5498-136">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="e5498-136">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="e5498-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e5498-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e5498-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5498-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e5498-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5498-139">Response</span></span>
<span data-ttu-id="e5498-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5498-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5498-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e5498-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5498-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5498-142">Request</span></span>
<span data-ttu-id="e5498-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5498-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign

Content-type: application/json
Content-length: 578

{
  "appProvisioningConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ],
  "iOSLobAppProvisioningConfigAssignments": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5498-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5498-144">Response</span></span>
<span data-ttu-id="e5498-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5498-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





