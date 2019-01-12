---
title: Действие getTargetedUsersAndDevices
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3530986f6e240d648b5383fc868e5ccdbe731e94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951168"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="b79bf-103">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="b79bf-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="b79bf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b79bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b79bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b79bf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b79bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b79bf-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b79bf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b79bf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b79bf-108">Prerequisites</span></span>
<span data-ttu-id="b79bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b79bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b79bf-111">Permission type</span></span>|<span data-ttu-id="b79bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b79bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b79bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b79bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b79bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b79bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b79bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b79bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79bf-116">Not supported.</span></span>|
|<span data-ttu-id="b79bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b79bf-117">Application</span></span>|<span data-ttu-id="b79bf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b79bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b79bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="b79bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b79bf-120">Request headers</span></span>
|<span data-ttu-id="b79bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b79bf-121">Header</span></span>|<span data-ttu-id="b79bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b79bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b79bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79bf-123">Authorization</span></span>|<span data-ttu-id="b79bf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b79bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b79bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b79bf-125">Accept</span></span>|<span data-ttu-id="b79bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b79bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79bf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b79bf-127">Request body</span></span>
<span data-ttu-id="b79bf-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b79bf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b79bf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b79bf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b79bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b79bf-130">Property</span></span>|<span data-ttu-id="b79bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b79bf-131">Type</span></span>|<span data-ttu-id="b79bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b79bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79bf-133">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="b79bf-133">deviceConfigurationIds</span></span>|<span data-ttu-id="b79bf-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b79bf-134">String collection</span></span>|<span data-ttu-id="b79bf-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b79bf-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b79bf-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b79bf-136">Response</span></span>
<span data-ttu-id="b79bf-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b79bf-137">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b79bf-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b79bf-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="b79bf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b79bf-139">Request</span></span>
<span data-ttu-id="b79bf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b79bf-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b79bf-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b79bf-141">Response</span></span>
<span data-ttu-id="b79bf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b79bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```





