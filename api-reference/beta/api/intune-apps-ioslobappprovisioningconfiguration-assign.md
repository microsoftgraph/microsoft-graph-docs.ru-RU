---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d29c095cdf90b63e580f657268b2c84b816c7299
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965111"
---
# <a name="assign-action"></a><span data-ttu-id="48816-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="48816-103">assign action</span></span>

> <span data-ttu-id="48816-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48816-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48816-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48816-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48816-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="48816-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48816-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48816-107">Prerequisites</span></span>
<span data-ttu-id="48816-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48816-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48816-110">Permission type</span></span>|<span data-ttu-id="48816-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48816-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48816-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48816-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48816-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48816-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48816-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48816-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48816-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48816-115">Not supported.</span></span>|
|<span data-ttu-id="48816-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48816-116">Application</span></span>|<span data-ttu-id="48816-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48816-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48816-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48816-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="48816-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48816-119">Request headers</span></span>
|<span data-ttu-id="48816-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48816-120">Header</span></span>|<span data-ttu-id="48816-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48816-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48816-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48816-122">Authorization</span></span>|<span data-ttu-id="48816-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48816-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48816-124">Accept</span><span class="sxs-lookup"><span data-stu-id="48816-124">Accept</span></span>|<span data-ttu-id="48816-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48816-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48816-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48816-126">Request body</span></span>
<span data-ttu-id="48816-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48816-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="48816-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="48816-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="48816-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="48816-129">Property</span></span>|<span data-ttu-id="48816-130">Тип</span><span class="sxs-lookup"><span data-stu-id="48816-130">Type</span></span>|<span data-ttu-id="48816-131">Описание</span><span class="sxs-lookup"><span data-stu-id="48816-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48816-132">Апппровисионингконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="48816-132">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="48816-133">Коллекция [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48816-133">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="48816-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="48816-134">Not yet documented</span></span>|
|<span data-ttu-id="48816-135">Иослобапппровисионингконфигассигнментс</span><span class="sxs-lookup"><span data-stu-id="48816-135">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="48816-136">Коллекция [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48816-136">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="48816-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="48816-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="48816-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="48816-138">Response</span></span>
<span data-ttu-id="48816-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48816-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48816-140">Пример</span><span class="sxs-lookup"><span data-stu-id="48816-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="48816-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="48816-141">Request</span></span>
<span data-ttu-id="48816-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48816-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48816-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="48816-143">Response</span></span>
<span data-ttu-id="48816-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48816-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





