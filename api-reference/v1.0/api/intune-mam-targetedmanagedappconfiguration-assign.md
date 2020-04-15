---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4726b9ead55e146a65278035178afa82515c717
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43398229"
---
# <a name="assign-action"></a><span data-ttu-id="04b4f-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="04b4f-103">assign action</span></span>

<span data-ttu-id="04b4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04b4f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04b4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b4f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="04b4f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b4f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04b4f-107">Prerequisites</span></span>
<span data-ttu-id="04b4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b4f-110">Permission type</span></span>|<span data-ttu-id="04b4f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b4f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04b4f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b4f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04b4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b4f-115">Not supported.</span></span>|
|<span data-ttu-id="04b4f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b4f-116">Application</span></span>|<span data-ttu-id="04b4f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b4f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="04b4f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04b4f-119">Request headers</span></span>
|<span data-ttu-id="04b4f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04b4f-120">Header</span></span>|<span data-ttu-id="04b4f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04b4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b4f-122">Authorization</span></span>|<span data-ttu-id="04b4f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b4f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04b4f-124">Accept</span></span>|<span data-ttu-id="04b4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04b4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b4f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04b4f-126">Request body</span></span>
<span data-ttu-id="04b4f-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04b4f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04b4f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="04b4f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04b4f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="04b4f-129">Property</span></span>|<span data-ttu-id="04b4f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04b4f-130">Type</span></span>|<span data-ttu-id="04b4f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04b4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b4f-132">assignments</span><span class="sxs-lookup"><span data-stu-id="04b4f-132">assignments</span></span>|<span data-ttu-id="04b4f-133">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="04b4f-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="04b4f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04b4f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="04b4f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="04b4f-135">Response</span></span>
<span data-ttu-id="04b4f-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04b4f-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04b4f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="04b4f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b4f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b4f-138">Request</span></span>
<span data-ttu-id="04b4f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b4f-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="04b4f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b4f-140">Response</span></span>
<span data-ttu-id="04b4f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04b4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






