---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5a1177d5d6e8a7df83623d4efacd109947b220e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964124"
---
# <a name="assign-action"></a><span data-ttu-id="a5552-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="a5552-103">assign action</span></span>

> <span data-ttu-id="a5552-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5552-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5552-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5552-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5552-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5552-107">Prerequisites</span></span>
<span data-ttu-id="a5552-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5552-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5552-110">Permission type</span></span>|<span data-ttu-id="a5552-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5552-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5552-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5552-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5552-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5552-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5552-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5552-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5552-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5552-115">Not supported.</span></span>|
|<span data-ttu-id="a5552-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5552-116">Application</span></span>|<span data-ttu-id="a5552-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5552-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5552-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5552-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="a5552-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5552-119">Request headers</span></span>
|<span data-ttu-id="a5552-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5552-120">Header</span></span>|<span data-ttu-id="a5552-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5552-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5552-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5552-122">Authorization</span></span>|<span data-ttu-id="a5552-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5552-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5552-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5552-124">Accept</span></span>|<span data-ttu-id="a5552-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5552-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5552-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5552-126">Request body</span></span>
<span data-ttu-id="a5552-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5552-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5552-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a5552-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5552-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5552-129">Property</span></span>|<span data-ttu-id="a5552-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5552-130">Type</span></span>|<span data-ttu-id="a5552-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5552-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5552-132">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="a5552-132">mobileAppAssignments</span></span>|<span data-ttu-id="a5552-133">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a5552-133">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="a5552-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a5552-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5552-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5552-135">Response</span></span>
<span data-ttu-id="a5552-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5552-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5552-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a5552-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5552-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5552-138">Request</span></span>
<span data-ttu-id="a5552-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5552-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5552-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5552-140">Response</span></span>
<span data-ttu-id="a5552-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




