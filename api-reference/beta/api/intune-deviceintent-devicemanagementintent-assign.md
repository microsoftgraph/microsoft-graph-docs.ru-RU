---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06489ea973f8433269c16af1067008ddfd6e839a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177256"
---
# <a name="assign-action"></a><span data-ttu-id="15805-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="15805-103">assign action</span></span>

<span data-ttu-id="15805-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15805-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15805-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15805-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15805-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15805-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15805-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="15805-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15805-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15805-108">Prerequisites</span></span>
<span data-ttu-id="15805-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15805-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15805-111">Permission type</span></span>|<span data-ttu-id="15805-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15805-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15805-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15805-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15805-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15805-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15805-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15805-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15805-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15805-116">Not supported.</span></span>|
|<span data-ttu-id="15805-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15805-117">Application</span></span>|<span data-ttu-id="15805-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15805-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15805-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15805-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="15805-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15805-120">Request headers</span></span>
|<span data-ttu-id="15805-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15805-121">Header</span></span>|<span data-ttu-id="15805-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15805-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15805-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15805-123">Authorization</span></span>|<span data-ttu-id="15805-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15805-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15805-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15805-125">Accept</span></span>|<span data-ttu-id="15805-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15805-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15805-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15805-127">Request body</span></span>
<span data-ttu-id="15805-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15805-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15805-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="15805-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15805-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15805-130">Property</span></span>|<span data-ttu-id="15805-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15805-131">Type</span></span>|<span data-ttu-id="15805-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15805-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15805-133">assignments</span><span class="sxs-lookup"><span data-stu-id="15805-133">assignments</span></span>|<span data-ttu-id="15805-134">Коллекция [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="15805-134">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="15805-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15805-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15805-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="15805-136">Response</span></span>
<span data-ttu-id="15805-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15805-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15805-138">Пример</span><span class="sxs-lookup"><span data-stu-id="15805-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="15805-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="15805-139">Request</span></span>
<span data-ttu-id="15805-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15805-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assign

Content-type: application/json
Content-length: 268

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="15805-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="15805-141">Response</span></span>
<span data-ttu-id="15805-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15805-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



