---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f929e9c2d07ac22cbbce72333b8eea1847f8570
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538359"
---
# <a name="assign-action"></a><span data-ttu-id="5096c-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="5096c-103">assign action</span></span>

> <span data-ttu-id="5096c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5096c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5096c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5096c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5096c-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5096c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5096c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5096c-107">Prerequisites</span></span>
<span data-ttu-id="5096c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5096c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5096c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5096c-110">Permission type</span></span>|<span data-ttu-id="5096c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5096c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5096c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5096c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5096c-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="5096c-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="5096c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5096c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5096c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5096c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5096c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5096c-116">Not supported.</span></span>|
|<span data-ttu-id="5096c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5096c-117">Application</span></span>||
| <span data-ttu-id="5096c-118">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="5096c-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="5096c-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5096c-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5096c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5096c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5096c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5096c-121">Request headers</span></span>
|<span data-ttu-id="5096c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5096c-122">Header</span></span>|<span data-ttu-id="5096c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5096c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5096c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5096c-124">Authorization</span></span>|<span data-ttu-id="5096c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5096c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5096c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5096c-126">Accept</span></span>|<span data-ttu-id="5096c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5096c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5096c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5096c-128">Request body</span></span>
<span data-ttu-id="5096c-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5096c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5096c-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5096c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5096c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="5096c-131">Property</span></span>|<span data-ttu-id="5096c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5096c-132">Type</span></span>|<span data-ttu-id="5096c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5096c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5096c-134">апппровисионингконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="5096c-134">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="5096c-135">Коллекция [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5096c-135">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="5096c-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5096c-136">Not yet documented</span></span>|
|<span data-ttu-id="5096c-137">иослобапппровисионингконфигассигнментс</span><span class="sxs-lookup"><span data-stu-id="5096c-137">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="5096c-138">Коллекция [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5096c-138">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5096c-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5096c-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5096c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="5096c-140">Response</span></span>
<span data-ttu-id="5096c-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5096c-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5096c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="5096c-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="5096c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="5096c-143">Request</span></span>
<span data-ttu-id="5096c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5096c-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5096c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5096c-145">Response</span></span>
<span data-ttu-id="5096c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5096c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






