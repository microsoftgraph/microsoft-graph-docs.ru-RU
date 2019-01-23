---
title: Действие getTargetedUsersAndDevices
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ec15ceb57e0e3142152ad7631f70495d2215dd3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412004"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="f72e1-103">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="f72e1-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="f72e1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f72e1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f72e1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f72e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f72e1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f72e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f72e1-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f72e1-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f72e1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f72e1-108">Prerequisites</span></span>
<span data-ttu-id="f72e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f72e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f72e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f72e1-111">Permission type</span></span>|<span data-ttu-id="f72e1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f72e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f72e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f72e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f72e1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f72e1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f72e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f72e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f72e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f72e1-116">Not supported.</span></span>|
|<span data-ttu-id="f72e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f72e1-117">Application</span></span>|<span data-ttu-id="f72e1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f72e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f72e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f72e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="f72e1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f72e1-120">Request headers</span></span>
|<span data-ttu-id="f72e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f72e1-121">Header</span></span>|<span data-ttu-id="f72e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f72e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f72e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f72e1-123">Authorization</span></span>|<span data-ttu-id="f72e1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f72e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f72e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f72e1-125">Accept</span></span>|<span data-ttu-id="f72e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f72e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f72e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f72e1-127">Request body</span></span>
<span data-ttu-id="f72e1-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f72e1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f72e1-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f72e1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f72e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f72e1-130">Property</span></span>|<span data-ttu-id="f72e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f72e1-131">Type</span></span>|<span data-ttu-id="f72e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f72e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f72e1-133">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="f72e1-133">deviceConfigurationIds</span></span>|<span data-ttu-id="f72e1-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f72e1-134">String collection</span></span>|<span data-ttu-id="f72e1-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f72e1-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f72e1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f72e1-136">Response</span></span>
<span data-ttu-id="f72e1-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f72e1-137">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f72e1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f72e1-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f72e1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f72e1-139">Request</span></span>
<span data-ttu-id="f72e1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f72e1-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f72e1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f72e1-141">Response</span></span>
<span data-ttu-id="f72e1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f72e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




