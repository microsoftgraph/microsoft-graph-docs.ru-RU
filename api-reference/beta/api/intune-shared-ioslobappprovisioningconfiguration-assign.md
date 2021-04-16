---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b9e31c360eec26c40c326f0b472034b10e86f3f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867730"
---
# <a name="assign-action"></a><span data-ttu-id="f10f0-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="f10f0-103">assign action</span></span>

<span data-ttu-id="f10f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f10f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f10f0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f10f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f10f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10f0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f10f0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f10f0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f10f0-108">Prerequisites</span></span>
<span data-ttu-id="f10f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f10f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f10f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f10f0-111">Permission type</span></span>|<span data-ttu-id="f10f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f10f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f10f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f10f0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f10f0-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="f10f0-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f10f0-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10f0-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f10f0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f10f0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f10f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10f0-117">Not supported.</span></span>|
|<span data-ttu-id="f10f0-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f10f0-118">Application</span></span>||
| <span data-ttu-id="f10f0-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="f10f0-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f10f0-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10f0-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f10f0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f10f0-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f10f0-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f10f0-122">Request headers</span></span>
|<span data-ttu-id="f10f0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f10f0-123">Header</span></span>|<span data-ttu-id="f10f0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f10f0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f10f0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f10f0-125">Authorization</span></span>|<span data-ttu-id="f10f0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f10f0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f10f0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f10f0-127">Accept</span></span>|<span data-ttu-id="f10f0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f10f0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10f0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f10f0-129">Request body</span></span>
<span data-ttu-id="f10f0-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f10f0-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f10f0-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f10f0-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f10f0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f10f0-132">Property</span></span>|<span data-ttu-id="f10f0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f10f0-133">Type</span></span>|<span data-ttu-id="f10f0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f10f0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10f0-135">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="f10f0-135">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="f10f0-136">[коллекция mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f10f0-136">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="f10f0-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f10f0-137">Not yet documented</span></span>|
|<span data-ttu-id="f10f0-138">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="f10f0-138">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="f10f0-139">[коллекция iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f10f0-139">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f10f0-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f10f0-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f10f0-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f10f0-141">Response</span></span>
<span data-ttu-id="f10f0-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f10f0-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f10f0-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f10f0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f10f0-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f10f0-144">Request</span></span>
<span data-ttu-id="f10f0-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f10f0-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f10f0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f10f0-146">Response</span></span>
<span data-ttu-id="f10f0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f10f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







