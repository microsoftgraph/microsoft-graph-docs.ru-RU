---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88687c6d1a082ab43f87fae701234392f2c8e096
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085607"
---
# <a name="assign-action"></a><span data-ttu-id="a4bab-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="a4bab-103">assign action</span></span>

<span data-ttu-id="a4bab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4bab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4bab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4bab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4bab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4bab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4bab-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a4bab-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4bab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4bab-108">Prerequisites</span></span>
<span data-ttu-id="a4bab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4bab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bab-111">Permission type</span></span>|<span data-ttu-id="a4bab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4bab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4bab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4bab-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a4bab-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a4bab-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a4bab-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4bab-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4bab-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4bab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4bab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4bab-117">Not supported.</span></span>|
|<span data-ttu-id="a4bab-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4bab-118">Application</span></span>||
| <span data-ttu-id="a4bab-119">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a4bab-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a4bab-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4bab-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4bab-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4bab-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a4bab-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4bab-122">Request headers</span></span>
|<span data-ttu-id="a4bab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4bab-123">Header</span></span>|<span data-ttu-id="a4bab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a4bab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4bab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4bab-125">Authorization</span></span>|<span data-ttu-id="a4bab-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4bab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4bab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a4bab-127">Accept</span></span>|<span data-ttu-id="a4bab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4bab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4bab-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4bab-129">Request body</span></span>
<span data-ttu-id="a4bab-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4bab-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a4bab-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a4bab-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a4bab-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4bab-132">Property</span></span>|<span data-ttu-id="a4bab-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a4bab-133">Type</span></span>|<span data-ttu-id="a4bab-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a4bab-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4bab-135">assignments</span><span class="sxs-lookup"><span data-stu-id="a4bab-135">assignments</span></span>|<span data-ttu-id="a4bab-136">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a4bab-136">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a4bab-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a4bab-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a4bab-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4bab-138">Response</span></span>
<span data-ttu-id="a4bab-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4bab-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4bab-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a4bab-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4bab-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4bab-141">Request</span></span>
<span data-ttu-id="a4bab-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4bab-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4bab-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bab-143">Response</span></span>
<span data-ttu-id="a4bab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4bab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









