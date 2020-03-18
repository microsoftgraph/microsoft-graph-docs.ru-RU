---
title: Действие assign
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f83ec3e1cddbc7a4ba5fc4f513656872f72f4ba5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800811"
---
# <a name="assign-action"></a><span data-ttu-id="89b1f-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="89b1f-103">assign action</span></span>

> <span data-ttu-id="89b1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89b1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89b1f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89b1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89b1f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="89b1f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89b1f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89b1f-107">Prerequisites</span></span>
<span data-ttu-id="89b1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89b1f-110">Permission type</span></span>|<span data-ttu-id="89b1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89b1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89b1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89b1f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="89b1f-113">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="89b1f-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="89b1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89b1f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89b1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89b1f-116">Not supported.</span></span>|
|<span data-ttu-id="89b1f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="89b1f-117">Application</span></span>||
| <span data-ttu-id="89b1f-118">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="89b1f-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="89b1f-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b1f-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89b1f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89b1f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="89b1f-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89b1f-121">Request headers</span></span>
|<span data-ttu-id="89b1f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89b1f-122">Header</span></span>|<span data-ttu-id="89b1f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="89b1f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89b1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89b1f-124">Authorization</span></span>|<span data-ttu-id="89b1f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89b1f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89b1f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="89b1f-126">Accept</span></span>|<span data-ttu-id="89b1f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89b1f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89b1f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89b1f-128">Request body</span></span>
<span data-ttu-id="89b1f-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89b1f-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="89b1f-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="89b1f-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="89b1f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="89b1f-131">Property</span></span>|<span data-ttu-id="89b1f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="89b1f-132">Type</span></span>|<span data-ttu-id="89b1f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="89b1f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b1f-134">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="89b1f-134">mobileAppAssignments</span></span>|<span data-ttu-id="89b1f-135">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89b1f-135">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="89b1f-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="89b1f-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89b1f-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="89b1f-137">Response</span></span>
<span data-ttu-id="89b1f-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="89b1f-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="89b1f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="89b1f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="89b1f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="89b1f-140">Request</span></span>
<span data-ttu-id="89b1f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89b1f-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89b1f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="89b1f-142">Response</span></span>
<span data-ttu-id="89b1f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89b1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







