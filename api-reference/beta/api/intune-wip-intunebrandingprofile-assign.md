---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 215052bb80669acb5f7ba450dfc93816e1d02111
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709070"
---
# <a name="assign-action"></a><span data-ttu-id="9c194-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="9c194-103">assign action</span></span>

<span data-ttu-id="9c194-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c194-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c194-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c194-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c194-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c194-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c194-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9c194-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c194-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9c194-108">Prerequisites</span></span>
<span data-ttu-id="9c194-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c194-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c194-111">Permission type</span></span>|<span data-ttu-id="9c194-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c194-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c194-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c194-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c194-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c194-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c194-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c194-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c194-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c194-116">Not supported.</span></span>|
|<span data-ttu-id="9c194-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c194-117">Application</span></span>|<span data-ttu-id="9c194-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c194-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c194-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c194-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9c194-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c194-120">Request headers</span></span>
|<span data-ttu-id="9c194-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c194-121">Header</span></span>|<span data-ttu-id="9c194-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c194-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c194-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c194-123">Authorization</span></span>|<span data-ttu-id="9c194-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c194-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c194-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c194-125">Accept</span></span>|<span data-ttu-id="9c194-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c194-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c194-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c194-127">Request body</span></span>
<span data-ttu-id="9c194-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c194-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9c194-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9c194-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9c194-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c194-130">Property</span></span>|<span data-ttu-id="9c194-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9c194-131">Type</span></span>|<span data-ttu-id="9c194-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9c194-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c194-133">assignments</span><span class="sxs-lookup"><span data-stu-id="9c194-133">assignments</span></span>|<span data-ttu-id="9c194-134">Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9c194-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="9c194-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9c194-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c194-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c194-136">Response</span></span>
<span data-ttu-id="9c194-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c194-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c194-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9c194-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c194-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c194-139">Request</span></span>
<span data-ttu-id="9c194-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c194-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 442

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9c194-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c194-141">Response</span></span>
<span data-ttu-id="9c194-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c194-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





