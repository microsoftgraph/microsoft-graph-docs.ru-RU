---
title: Действие assign
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 037dd1299c4c6fb23ca567d9607dd1d77f5259c0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729649"
---
# <a name="assign-action"></a><span data-ttu-id="c8292-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="c8292-103">assign action</span></span>

> <span data-ttu-id="c8292-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8292-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8292-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8292-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8292-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c8292-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8292-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8292-107">Prerequisites</span></span>
<span data-ttu-id="c8292-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8292-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8292-110">Permission type</span></span>|<span data-ttu-id="c8292-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8292-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8292-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8292-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8292-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8292-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8292-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8292-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8292-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8292-115">Not supported.</span></span>|
|<span data-ttu-id="c8292-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8292-116">Application</span></span>|<span data-ttu-id="c8292-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8292-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8292-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8292-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c8292-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8292-119">Request headers</span></span>
|<span data-ttu-id="c8292-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8292-120">Header</span></span>|<span data-ttu-id="c8292-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c8292-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8292-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8292-122">Authorization</span></span>|<span data-ttu-id="c8292-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8292-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8292-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c8292-124">Accept</span></span>|<span data-ttu-id="c8292-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8292-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8292-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8292-126">Request body</span></span>
<span data-ttu-id="c8292-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8292-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c8292-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c8292-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c8292-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8292-129">Property</span></span>|<span data-ttu-id="c8292-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c8292-130">Type</span></span>|<span data-ttu-id="c8292-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c8292-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8292-132">assignments</span><span class="sxs-lookup"><span data-stu-id="c8292-132">assignments</span></span>|<span data-ttu-id="c8292-133">Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c8292-133">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="c8292-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c8292-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c8292-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8292-135">Response</span></span>
<span data-ttu-id="c8292-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8292-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8292-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c8292-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8292-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8292-138">Request</span></span>
<span data-ttu-id="c8292-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8292-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8292-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8292-140">Response</span></span>
<span data-ttu-id="c8292-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




