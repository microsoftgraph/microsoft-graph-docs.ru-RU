---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8917c1ec61104584136f329e64c578fd9f55a87
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201166"
---
# <a name="assign-action"></a><span data-ttu-id="c9370-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="c9370-103">assign action</span></span>

> <span data-ttu-id="c9370-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9370-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9370-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9370-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9370-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c9370-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9370-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9370-107">Prerequisites</span></span>
<span data-ttu-id="c9370-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9370-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9370-110">Permission type</span></span>|<span data-ttu-id="c9370-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9370-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9370-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9370-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9370-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="c9370-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c9370-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9370-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9370-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9370-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9370-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9370-116">Not supported.</span></span>|
|<span data-ttu-id="c9370-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9370-117">Application</span></span>||
| <span data-ttu-id="c9370-118">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="c9370-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c9370-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9370-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9370-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9370-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="c9370-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9370-121">Request headers</span></span>
|<span data-ttu-id="c9370-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9370-122">Header</span></span>|<span data-ttu-id="c9370-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c9370-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9370-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9370-124">Authorization</span></span>|<span data-ttu-id="c9370-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9370-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9370-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c9370-126">Accept</span></span>|<span data-ttu-id="c9370-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c9370-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9370-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9370-128">Request body</span></span>
<span data-ttu-id="c9370-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9370-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c9370-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c9370-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c9370-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9370-131">Property</span></span>|<span data-ttu-id="c9370-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c9370-132">Type</span></span>|<span data-ttu-id="c9370-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c9370-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9370-134">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="c9370-134">mobileAppAssignments</span></span>|<span data-ttu-id="c9370-135">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9370-135">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c9370-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c9370-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c9370-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9370-137">Response</span></span>
<span data-ttu-id="c9370-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9370-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9370-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c9370-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9370-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9370-140">Request</span></span>
<span data-ttu-id="c9370-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9370-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9370-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9370-142">Response</span></span>
<span data-ttu-id="c9370-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9370-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




