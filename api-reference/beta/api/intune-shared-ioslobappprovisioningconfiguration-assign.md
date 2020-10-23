---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df2bc820f99d7e2ce324c24c1a9b8e782cc60fba
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691591"
---
# <a name="assign-action"></a><span data-ttu-id="089d8-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="089d8-103">assign action</span></span>

<span data-ttu-id="089d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="089d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="089d8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="089d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="089d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089d8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="089d8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="089d8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="089d8-108">Prerequisites</span></span>
<span data-ttu-id="089d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="089d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="089d8-111">Permission type</span></span>|<span data-ttu-id="089d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="089d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="089d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="089d8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="089d8-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="089d8-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="089d8-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089d8-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="089d8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="089d8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="089d8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089d8-117">Not supported.</span></span>|
|<span data-ttu-id="089d8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="089d8-118">Application</span></span>||
| <span data-ttu-id="089d8-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="089d8-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="089d8-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089d8-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="089d8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="089d8-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="089d8-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="089d8-122">Request headers</span></span>
|<span data-ttu-id="089d8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="089d8-123">Header</span></span>|<span data-ttu-id="089d8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="089d8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="089d8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="089d8-125">Authorization</span></span>|<span data-ttu-id="089d8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="089d8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="089d8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="089d8-127">Accept</span></span>|<span data-ttu-id="089d8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="089d8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="089d8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="089d8-129">Request body</span></span>
<span data-ttu-id="089d8-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="089d8-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="089d8-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="089d8-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="089d8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="089d8-132">Property</span></span>|<span data-ttu-id="089d8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="089d8-133">Type</span></span>|<span data-ttu-id="089d8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="089d8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089d8-135">апппровисионингконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="089d8-135">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="089d8-136">Коллекция [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="089d8-136">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="089d8-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="089d8-137">Not yet documented</span></span>|
|<span data-ttu-id="089d8-138">иослобапппровисионингконфигассигнментс</span><span class="sxs-lookup"><span data-stu-id="089d8-138">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="089d8-139">Коллекция [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="089d8-139">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="089d8-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="089d8-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="089d8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="089d8-141">Response</span></span>
<span data-ttu-id="089d8-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="089d8-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="089d8-143">Пример</span><span class="sxs-lookup"><span data-stu-id="089d8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="089d8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="089d8-144">Request</span></span>
<span data-ttu-id="089d8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="089d8-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="089d8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="089d8-146">Response</span></span>
<span data-ttu-id="089d8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="089d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








