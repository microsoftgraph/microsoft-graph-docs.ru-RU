---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83ca25deefb192bfef2bcc5ed260e450bfc8cf59
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133866"
---
# <a name="assign-action"></a><span data-ttu-id="e363d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e363d-103">assign action</span></span>

<span data-ttu-id="e363d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e363d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e363d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e363d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e363d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e363d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e363d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e363d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e363d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e363d-108">Prerequisites</span></span>
<span data-ttu-id="e363d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e363d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e363d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e363d-111">Permission type</span></span>|<span data-ttu-id="e363d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e363d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e363d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e363d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e363d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e363d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e363d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e363d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e363d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e363d-116">Not supported.</span></span>|
|<span data-ttu-id="e363d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e363d-117">Application</span></span>|<span data-ttu-id="e363d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e363d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e363d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e363d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e363d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e363d-120">Request headers</span></span>
|<span data-ttu-id="e363d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e363d-121">Header</span></span>|<span data-ttu-id="e363d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e363d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e363d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e363d-123">Authorization</span></span>|<span data-ttu-id="e363d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e363d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e363d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e363d-125">Accept</span></span>|<span data-ttu-id="e363d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e363d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e363d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e363d-127">Request body</span></span>
<span data-ttu-id="e363d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e363d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e363d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e363d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e363d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e363d-130">Property</span></span>|<span data-ttu-id="e363d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e363d-131">Type</span></span>|<span data-ttu-id="e363d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e363d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e363d-133">assignments</span><span class="sxs-lookup"><span data-stu-id="e363d-133">assignments</span></span>|<span data-ttu-id="e363d-134">[коллекция intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e363d-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="e363d-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e363d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e363d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e363d-136">Response</span></span>
<span data-ttu-id="e363d-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e363d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e363d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e363d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e363d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e363d-139">Request</span></span>
<span data-ttu-id="e363d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e363d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 510

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
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

### <a name="response"></a><span data-ttu-id="e363d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e363d-141">Response</span></span>
<span data-ttu-id="e363d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e363d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




