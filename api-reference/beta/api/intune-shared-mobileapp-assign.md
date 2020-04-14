---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0db9650decfd563415860a6a563a6cda66e869f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448669"
---
# <a name="assign-action"></a><span data-ttu-id="0d694-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="0d694-103">assign action</span></span>

<span data-ttu-id="0d694-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d694-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d694-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d694-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d694-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0d694-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d694-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d694-108">Prerequisites</span></span>
<span data-ttu-id="0d694-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d694-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d694-111">Permission type</span></span>|<span data-ttu-id="0d694-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d694-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d694-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d694-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0d694-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="0d694-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="0d694-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d694-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d694-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d694-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d694-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d694-117">Not supported.</span></span>|
|<span data-ttu-id="0d694-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d694-118">Application</span></span>||
| <span data-ttu-id="0d694-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="0d694-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="0d694-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d694-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d694-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d694-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="0d694-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d694-122">Request headers</span></span>
|<span data-ttu-id="0d694-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d694-123">Header</span></span>|<span data-ttu-id="0d694-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0d694-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d694-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d694-125">Authorization</span></span>|<span data-ttu-id="0d694-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d694-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d694-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0d694-127">Accept</span></span>|<span data-ttu-id="0d694-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d694-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d694-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d694-129">Request body</span></span>
<span data-ttu-id="0d694-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d694-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0d694-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0d694-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0d694-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d694-132">Property</span></span>|<span data-ttu-id="0d694-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0d694-133">Type</span></span>|<span data-ttu-id="0d694-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0d694-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d694-135">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="0d694-135">mobileAppAssignments</span></span>|<span data-ttu-id="0d694-136">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0d694-136">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="0d694-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0d694-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0d694-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d694-138">Response</span></span>
<span data-ttu-id="0d694-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d694-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d694-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0d694-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d694-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d694-141">Request</span></span>
<span data-ttu-id="0d694-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d694-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0d694-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d694-143">Response</span></span>
<span data-ttu-id="0d694-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d694-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






