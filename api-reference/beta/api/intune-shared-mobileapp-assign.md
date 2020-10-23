---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62411150b8fc309db053e0604c65a4fd3213fa5d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729891"
---
# <a name="assign-action"></a><span data-ttu-id="52420-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="52420-103">assign action</span></span>

<span data-ttu-id="52420-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52420-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52420-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52420-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52420-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52420-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52420-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="52420-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52420-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52420-108">Prerequisites</span></span>
<span data-ttu-id="52420-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52420-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52420-111">Permission type</span></span>|<span data-ttu-id="52420-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52420-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52420-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52420-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="52420-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="52420-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="52420-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52420-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52420-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52420-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52420-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52420-117">Not supported.</span></span>|
|<span data-ttu-id="52420-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52420-118">Application</span></span>||
| <span data-ttu-id="52420-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="52420-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="52420-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52420-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52420-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52420-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="52420-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52420-122">Request headers</span></span>
|<span data-ttu-id="52420-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52420-123">Header</span></span>|<span data-ttu-id="52420-124">Значение</span><span class="sxs-lookup"><span data-stu-id="52420-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52420-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52420-125">Authorization</span></span>|<span data-ttu-id="52420-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52420-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52420-127">Accept</span><span class="sxs-lookup"><span data-stu-id="52420-127">Accept</span></span>|<span data-ttu-id="52420-128">application/json</span><span class="sxs-lookup"><span data-stu-id="52420-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52420-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52420-129">Request body</span></span>
<span data-ttu-id="52420-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52420-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="52420-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="52420-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="52420-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="52420-132">Property</span></span>|<span data-ttu-id="52420-133">Тип</span><span class="sxs-lookup"><span data-stu-id="52420-133">Type</span></span>|<span data-ttu-id="52420-134">Описание</span><span class="sxs-lookup"><span data-stu-id="52420-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52420-135">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="52420-135">mobileAppAssignments</span></span>|<span data-ttu-id="52420-136">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52420-136">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="52420-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="52420-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="52420-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="52420-138">Response</span></span>
<span data-ttu-id="52420-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52420-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52420-140">Пример</span><span class="sxs-lookup"><span data-stu-id="52420-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="52420-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="52420-141">Request</span></span>
<span data-ttu-id="52420-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52420-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52420-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="52420-143">Response</span></span>
<span data-ttu-id="52420-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52420-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








