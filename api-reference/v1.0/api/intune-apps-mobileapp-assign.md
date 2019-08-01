---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30d4ba44ba17dc2312a2379e3add1649f0389fc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013796"
---
# <a name="assign-action"></a><span data-ttu-id="d1e88-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="d1e88-103">assign action</span></span>

> <span data-ttu-id="d1e88-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1e88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e88-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1e88-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1e88-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1e88-106">Prerequisites</span></span>
<span data-ttu-id="d1e88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e88-109">Permission type</span></span>|<span data-ttu-id="d1e88-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1e88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1e88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1e88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e88-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e88-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1e88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1e88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1e88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e88-114">Not supported.</span></span>|
|<span data-ttu-id="d1e88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1e88-115">Application</span></span>|<span data-ttu-id="d1e88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1e88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1e88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d1e88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1e88-118">Request headers</span></span>
|<span data-ttu-id="d1e88-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1e88-119">Header</span></span>|<span data-ttu-id="d1e88-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d1e88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1e88-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1e88-121">Authorization</span></span>|<span data-ttu-id="d1e88-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1e88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1e88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d1e88-123">Accept</span></span>|<span data-ttu-id="d1e88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1e88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1e88-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1e88-125">Request body</span></span>
<span data-ttu-id="d1e88-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1e88-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d1e88-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d1e88-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d1e88-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1e88-128">Property</span></span>|<span data-ttu-id="d1e88-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d1e88-129">Type</span></span>|<span data-ttu-id="d1e88-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1e88-131">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="d1e88-131">mobileAppAssignments</span></span>|<span data-ttu-id="d1e88-132">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d1e88-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="d1e88-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d1e88-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d1e88-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1e88-134">Response</span></span>
<span data-ttu-id="d1e88-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1e88-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1e88-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d1e88-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1e88-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1e88-137">Request</span></span>
<span data-ttu-id="d1e88-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1e88-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

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

### <a name="response"></a><span data-ttu-id="d1e88-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e88-139">Response</span></span>
<span data-ttu-id="d1e88-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1e88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



