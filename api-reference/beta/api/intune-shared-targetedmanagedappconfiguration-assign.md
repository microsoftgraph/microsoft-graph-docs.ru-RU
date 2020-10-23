---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4799b3cd4bb6353e8ca0a297983ee4a1532f19ac
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698045"
---
# <a name="assign-action"></a><span data-ttu-id="0247d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="0247d-103">assign action</span></span>

<span data-ttu-id="0247d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0247d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0247d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0247d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0247d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0247d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0247d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0247d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0247d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0247d-108">Prerequisites</span></span>
<span data-ttu-id="0247d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0247d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0247d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0247d-111">Permission type</span></span>|<span data-ttu-id="0247d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0247d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0247d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0247d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0247d-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="0247d-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0247d-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0247d-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0247d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0247d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0247d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0247d-117">Not supported.</span></span>|
|<span data-ttu-id="0247d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0247d-118">Application</span></span>||
| <span data-ttu-id="0247d-119">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="0247d-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0247d-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0247d-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0247d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0247d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0247d-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0247d-122">Request headers</span></span>
|<span data-ttu-id="0247d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0247d-123">Header</span></span>|<span data-ttu-id="0247d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0247d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0247d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0247d-125">Authorization</span></span>|<span data-ttu-id="0247d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0247d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0247d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0247d-127">Accept</span></span>|<span data-ttu-id="0247d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0247d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0247d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0247d-129">Request body</span></span>
<span data-ttu-id="0247d-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0247d-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0247d-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0247d-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0247d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0247d-132">Property</span></span>|<span data-ttu-id="0247d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0247d-133">Type</span></span>|<span data-ttu-id="0247d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0247d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0247d-135">assignments</span><span class="sxs-lookup"><span data-stu-id="0247d-135">assignments</span></span>|<span data-ttu-id="0247d-136">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0247d-136">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="0247d-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0247d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0247d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0247d-138">Response</span></span>
<span data-ttu-id="0247d-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0247d-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0247d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0247d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0247d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0247d-141">Request</span></span>
<span data-ttu-id="0247d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0247d-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0247d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0247d-143">Response</span></span>
<span data-ttu-id="0247d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0247d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








