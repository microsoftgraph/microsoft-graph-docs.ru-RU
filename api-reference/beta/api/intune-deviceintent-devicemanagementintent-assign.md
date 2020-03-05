---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85ecb9c2f626f65936f55a57a148feec508be7d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471577"
---
# <a name="assign-action"></a><span data-ttu-id="63e13-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="63e13-103">assign action</span></span>

<span data-ttu-id="63e13-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="63e13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63e13-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63e13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63e13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63e13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e13-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="63e13-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63e13-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63e13-108">Prerequisites</span></span>
<span data-ttu-id="63e13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63e13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63e13-111">Permission type</span></span>|<span data-ttu-id="63e13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63e13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63e13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63e13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63e13-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e13-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63e13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63e13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63e13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63e13-116">Not supported.</span></span>|
|<span data-ttu-id="63e13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63e13-117">Application</span></span>|<span data-ttu-id="63e13-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e13-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63e13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63e13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="63e13-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63e13-120">Request headers</span></span>
|<span data-ttu-id="63e13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63e13-121">Header</span></span>|<span data-ttu-id="63e13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63e13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63e13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e13-123">Authorization</span></span>|<span data-ttu-id="63e13-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63e13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63e13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63e13-125">Accept</span></span>|<span data-ttu-id="63e13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63e13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e13-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63e13-127">Request body</span></span>
<span data-ttu-id="63e13-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63e13-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="63e13-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="63e13-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="63e13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63e13-130">Property</span></span>|<span data-ttu-id="63e13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63e13-131">Type</span></span>|<span data-ttu-id="63e13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63e13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e13-133">assignments</span><span class="sxs-lookup"><span data-stu-id="63e13-133">assignments</span></span>|<span data-ttu-id="63e13-134">Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63e13-134">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="63e13-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="63e13-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="63e13-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="63e13-136">Response</span></span>
<span data-ttu-id="63e13-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63e13-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63e13-138">Пример</span><span class="sxs-lookup"><span data-stu-id="63e13-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="63e13-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="63e13-139">Request</span></span>
<span data-ttu-id="63e13-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63e13-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="63e13-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="63e13-141">Response</span></span>
<span data-ttu-id="63e13-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63e13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





