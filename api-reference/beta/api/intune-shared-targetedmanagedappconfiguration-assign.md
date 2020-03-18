---
title: Действие assign
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76d80ce2ecf6b4501122ba35efac44f9c6e9af14
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800657"
---
# <a name="assign-action"></a><span data-ttu-id="9ffeb-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="9ffeb-103">assign action</span></span>

> <span data-ttu-id="9ffeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ffeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ffeb-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ffeb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ffeb-107">Prerequisites</span></span>
<span data-ttu-id="9ffeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ffeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ffeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ffeb-110">Permission type</span></span>|<span data-ttu-id="9ffeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ffeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ffeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ffeb-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9ffeb-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="9ffeb-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="9ffeb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffeb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ffeb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ffeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ffeb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-116">Not supported.</span></span>|
|<span data-ttu-id="9ffeb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ffeb-117">Application</span></span>||
| <span data-ttu-id="9ffeb-118">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="9ffeb-118">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="9ffeb-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffeb-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ffeb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ffeb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9ffeb-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ffeb-121">Request headers</span></span>
|<span data-ttu-id="9ffeb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ffeb-122">Header</span></span>|<span data-ttu-id="9ffeb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9ffeb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ffeb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ffeb-124">Authorization</span></span>|<span data-ttu-id="9ffeb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ffeb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9ffeb-126">Accept</span></span>|<span data-ttu-id="9ffeb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ffeb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ffeb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ffeb-128">Request body</span></span>
<span data-ttu-id="9ffeb-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9ffeb-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9ffeb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ffeb-131">Property</span></span>|<span data-ttu-id="9ffeb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9ffeb-132">Type</span></span>|<span data-ttu-id="9ffeb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9ffeb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ffeb-134">assignments</span><span class="sxs-lookup"><span data-stu-id="9ffeb-134">assignments</span></span>|<span data-ttu-id="9ffeb-135">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9ffeb-135">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9ffeb-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9ffeb-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9ffeb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ffeb-137">Response</span></span>
<span data-ttu-id="9ffeb-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ffeb-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9ffeb-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ffeb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ffeb-140">Request</span></span>
<span data-ttu-id="9ffeb-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 351

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9ffeb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ffeb-142">Response</span></span>
<span data-ttu-id="9ffeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ffeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







