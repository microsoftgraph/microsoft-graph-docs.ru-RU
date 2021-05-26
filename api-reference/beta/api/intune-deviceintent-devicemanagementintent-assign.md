---
title: Намерение управления устройствами назначить действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4594badde9c3088aeebc015c378ed660517f7c4c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666326"
---
# <a name="device-management-intent-assign-action"></a><span data-ttu-id="0e27a-103">Намерение управления устройствами назначить действие</span><span class="sxs-lookup"><span data-stu-id="0e27a-103">Device management intent assign action</span></span>

<span data-ttu-id="0e27a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e27a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e27a-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e27a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e27a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e27a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e27a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0e27a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e27a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e27a-108">Prerequisites</span></span>
<span data-ttu-id="0e27a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e27a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e27a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e27a-111">Permission type</span></span>|<span data-ttu-id="0e27a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e27a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e27a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e27a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e27a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e27a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e27a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e27a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e27a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e27a-116">Not supported.</span></span>|
|<span data-ttu-id="0e27a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e27a-117">Application</span></span>|<span data-ttu-id="0e27a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e27a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e27a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e27a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0e27a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e27a-120">Request headers</span></span>
|<span data-ttu-id="0e27a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e27a-121">Header</span></span>|<span data-ttu-id="0e27a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e27a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e27a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e27a-123">Authorization</span></span>|<span data-ttu-id="0e27a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e27a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e27a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e27a-125">Accept</span></span>|<span data-ttu-id="0e27a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e27a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e27a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e27a-127">Request body</span></span>
<span data-ttu-id="0e27a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e27a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0e27a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0e27a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0e27a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e27a-130">Property</span></span>|<span data-ttu-id="0e27a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e27a-131">Type</span></span>|<span data-ttu-id="0e27a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e27a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e27a-133">assignments</span><span class="sxs-lookup"><span data-stu-id="0e27a-133">assignments</span></span>|<span data-ttu-id="0e27a-134">[коллекция deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0e27a-134">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="0e27a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0e27a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e27a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e27a-136">Response</span></span>
<span data-ttu-id="0e27a-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e27a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e27a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0e27a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e27a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e27a-139">Request</span></span>
<span data-ttu-id="0e27a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e27a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assign

Content-type: application/json
Content-length: 511

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0e27a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e27a-141">Response</span></span>
<span data-ttu-id="0e27a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e27a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




