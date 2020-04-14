---
title: Действие targetApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7499d8f18774930b2e89e14b372424f3326bc3e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465295"
---
# <a name="targetapps-action"></a><span data-ttu-id="f6b43-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="f6b43-103">targetApps action</span></span>

<span data-ttu-id="f6b43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6b43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6b43-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6b43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6b43-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6b43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6b43-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6b43-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6b43-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6b43-108">Prerequisites</span></span>
<span data-ttu-id="f6b43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6b43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6b43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6b43-111">Permission type</span></span>|<span data-ttu-id="f6b43-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6b43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6b43-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6b43-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f6b43-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f6b43-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f6b43-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6b43-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6b43-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6b43-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6b43-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6b43-117">Not supported.</span></span>|
|<span data-ttu-id="f6b43-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6b43-118">Application</span></span>||
| <span data-ttu-id="f6b43-119">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f6b43-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f6b43-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6b43-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6b43-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6b43-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="f6b43-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6b43-122">Request headers</span></span>
|<span data-ttu-id="f6b43-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6b43-123">Header</span></span>|<span data-ttu-id="f6b43-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f6b43-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6b43-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6b43-125">Authorization</span></span>|<span data-ttu-id="f6b43-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6b43-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6b43-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f6b43-127">Accept</span></span>|<span data-ttu-id="f6b43-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f6b43-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6b43-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6b43-129">Request body</span></span>
<span data-ttu-id="f6b43-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6b43-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f6b43-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f6b43-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f6b43-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6b43-132">Property</span></span>|<span data-ttu-id="f6b43-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f6b43-133">Type</span></span>|<span data-ttu-id="f6b43-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f6b43-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6b43-135">apps</span><span class="sxs-lookup"><span data-stu-id="f6b43-135">apps</span></span>|<span data-ttu-id="f6b43-136">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6b43-136">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="f6b43-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f6b43-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6b43-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6b43-138">Response</span></span>
<span data-ttu-id="f6b43-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6b43-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6b43-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f6b43-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6b43-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6b43-141">Request</span></span>
<span data-ttu-id="f6b43-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6b43-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f6b43-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6b43-143">Response</span></span>
<span data-ttu-id="f6b43-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6b43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






