---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebe78e868f47eb789182656291ad7ea3378dd29c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996040"
---
# <a name="assign-action"></a><span data-ttu-id="e421a-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e421a-103">assign action</span></span>

<span data-ttu-id="e421a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e421a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e421a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e421a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e421a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e421a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e421a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e421a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e421a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e421a-108">Prerequisites</span></span>
<span data-ttu-id="e421a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e421a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e421a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e421a-111">Permission type</span></span>|<span data-ttu-id="e421a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e421a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e421a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e421a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e421a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e421a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e421a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e421a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e421a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e421a-116">Not supported.</span></span>|
|<span data-ttu-id="e421a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e421a-117">Application</span></span>|<span data-ttu-id="e421a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e421a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e421a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e421a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e421a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e421a-120">Request headers</span></span>
|<span data-ttu-id="e421a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e421a-121">Header</span></span>|<span data-ttu-id="e421a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e421a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e421a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e421a-123">Authorization</span></span>|<span data-ttu-id="e421a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e421a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e421a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e421a-125">Accept</span></span>|<span data-ttu-id="e421a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e421a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e421a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e421a-127">Request body</span></span>
<span data-ttu-id="e421a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e421a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e421a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e421a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e421a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e421a-130">Property</span></span>|<span data-ttu-id="e421a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e421a-131">Type</span></span>|<span data-ttu-id="e421a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e421a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e421a-133">assignments</span><span class="sxs-lookup"><span data-stu-id="e421a-133">assignments</span></span>|<span data-ttu-id="e421a-134">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e421a-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e421a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e421a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e421a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e421a-136">Response</span></span>
<span data-ttu-id="e421a-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e421a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e421a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e421a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e421a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e421a-139">Request</span></span>
<span data-ttu-id="e421a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e421a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 462

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e421a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e421a-141">Response</span></span>
<span data-ttu-id="e421a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e421a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






