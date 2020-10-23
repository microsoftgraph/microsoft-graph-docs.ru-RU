---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c65578fcdb553454ee4fc0e289d6b5a30b8172b0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721521"
---
# <a name="assign-action"></a><span data-ttu-id="63bda-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="63bda-103">assign action</span></span>

<span data-ttu-id="63bda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63bda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63bda-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63bda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63bda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63bda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63bda-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="63bda-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63bda-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63bda-108">Prerequisites</span></span>
<span data-ttu-id="63bda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63bda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63bda-111">Permission type</span></span>|<span data-ttu-id="63bda-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63bda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63bda-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63bda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63bda-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bda-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63bda-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63bda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63bda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63bda-116">Not supported.</span></span>|
|<span data-ttu-id="63bda-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63bda-117">Application</span></span>|<span data-ttu-id="63bda-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bda-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63bda-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63bda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy/assign
```

## <a name="request-headers"></a><span data-ttu-id="63bda-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63bda-120">Request headers</span></span>
|<span data-ttu-id="63bda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63bda-121">Header</span></span>|<span data-ttu-id="63bda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63bda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63bda-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63bda-123">Authorization</span></span>|<span data-ttu-id="63bda-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63bda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63bda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63bda-125">Accept</span></span>|<span data-ttu-id="63bda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63bda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63bda-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63bda-127">Request body</span></span>
<span data-ttu-id="63bda-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63bda-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="63bda-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="63bda-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="63bda-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63bda-130">Property</span></span>|<span data-ttu-id="63bda-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63bda-131">Type</span></span>|<span data-ttu-id="63bda-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63bda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63bda-133">вдакполициассигнментс</span><span class="sxs-lookup"><span data-stu-id="63bda-133">wdacPolicyAssignments</span></span>|<span data-ttu-id="63bda-134">Коллекция [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63bda-134">[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection</span></span>|<span data-ttu-id="63bda-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="63bda-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="63bda-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="63bda-136">Response</span></span>
<span data-ttu-id="63bda-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63bda-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63bda-138">Пример</span><span class="sxs-lookup"><span data-stu-id="63bda-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="63bda-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="63bda-139">Request</span></span>
<span data-ttu-id="63bda-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63bda-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign

Content-type: application/json
Content-length: 494

{
  "wdacPolicyAssignments": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="63bda-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="63bda-141">Response</span></span>
<span data-ttu-id="63bda-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63bda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





