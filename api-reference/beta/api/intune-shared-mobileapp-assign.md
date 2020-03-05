---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2421889f5efbe34b3a69b5ea9f689b0111255454
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458317"
---
# <a name="assign-action"></a><span data-ttu-id="e552a-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e552a-103">assign action</span></span>

<span data-ttu-id="e552a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e552a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e552a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e552a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e552a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e552a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e552a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e552a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e552a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e552a-108">Prerequisites</span></span>
<span data-ttu-id="e552a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e552a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e552a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e552a-111">Permission type</span></span>|<span data-ttu-id="e552a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e552a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e552a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e552a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e552a-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="e552a-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="e552a-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e552a-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e552a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e552a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e552a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e552a-117">Not supported.</span></span>|
|<span data-ttu-id="e552a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e552a-118">Application</span></span>||
| <span data-ttu-id="e552a-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="e552a-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="e552a-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e552a-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e552a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e552a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="e552a-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e552a-122">Request headers</span></span>
|<span data-ttu-id="e552a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e552a-123">Header</span></span>|<span data-ttu-id="e552a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e552a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e552a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e552a-125">Authorization</span></span>|<span data-ttu-id="e552a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e552a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e552a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e552a-127">Accept</span></span>|<span data-ttu-id="e552a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e552a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e552a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e552a-129">Request body</span></span>
<span data-ttu-id="e552a-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e552a-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e552a-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e552a-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e552a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e552a-132">Property</span></span>|<span data-ttu-id="e552a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e552a-133">Type</span></span>|<span data-ttu-id="e552a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e552a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e552a-135">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="e552a-135">mobileAppAssignments</span></span>|<span data-ttu-id="e552a-136">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e552a-136">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e552a-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e552a-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e552a-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e552a-138">Response</span></span>
<span data-ttu-id="e552a-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e552a-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e552a-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e552a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e552a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e552a-141">Request</span></span>
<span data-ttu-id="e552a-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e552a-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e552a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e552a-143">Response</span></span>
<span data-ttu-id="e552a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e552a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








