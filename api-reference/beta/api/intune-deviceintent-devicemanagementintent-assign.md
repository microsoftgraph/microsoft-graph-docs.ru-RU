---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f3927237b74436733e1c371e98873edc45425be
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792585"
---
# <a name="assign-action"></a><span data-ttu-id="227be-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="227be-103">assign action</span></span>

<span data-ttu-id="227be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="227be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="227be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="227be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="227be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227be-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="227be-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="227be-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="227be-108">Prerequisites</span></span>
<span data-ttu-id="227be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="227be-111">Permission type</span></span>|<span data-ttu-id="227be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="227be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="227be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="227be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="227be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="227be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="227be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="227be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227be-116">Not supported.</span></span>|
|<span data-ttu-id="227be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="227be-117">Application</span></span>|<span data-ttu-id="227be-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227be-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="227be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="227be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="227be-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="227be-120">Request headers</span></span>
|<span data-ttu-id="227be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="227be-121">Header</span></span>|<span data-ttu-id="227be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="227be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="227be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="227be-123">Authorization</span></span>|<span data-ttu-id="227be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="227be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="227be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="227be-125">Accept</span></span>|<span data-ttu-id="227be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="227be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="227be-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="227be-127">Request body</span></span>
<span data-ttu-id="227be-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="227be-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="227be-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="227be-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="227be-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="227be-130">Property</span></span>|<span data-ttu-id="227be-131">Тип</span><span class="sxs-lookup"><span data-stu-id="227be-131">Type</span></span>|<span data-ttu-id="227be-132">Описание</span><span class="sxs-lookup"><span data-stu-id="227be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227be-133">assignments</span><span class="sxs-lookup"><span data-stu-id="227be-133">assignments</span></span>|<span data-ttu-id="227be-134">Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="227be-134">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="227be-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="227be-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="227be-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="227be-136">Response</span></span>
<span data-ttu-id="227be-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="227be-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="227be-138">Пример</span><span class="sxs-lookup"><span data-stu-id="227be-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="227be-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="227be-139">Request</span></span>
<span data-ttu-id="227be-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="227be-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assign

Content-type: application/json
Content-length: 443

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="227be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="227be-141">Response</span></span>
<span data-ttu-id="227be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="227be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



