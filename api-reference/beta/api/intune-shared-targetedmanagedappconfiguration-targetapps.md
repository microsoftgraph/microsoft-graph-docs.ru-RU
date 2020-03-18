---
title: Действие targetApps
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04e13d90392f5f83abfc4c17137f1e173a026f86
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800615"
---
# <a name="targetapps-action"></a><span data-ttu-id="d6674-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="d6674-103">targetApps action</span></span>

> <span data-ttu-id="d6674-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6674-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6674-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6674-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6674-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6674-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6674-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6674-107">Prerequisites</span></span>
<span data-ttu-id="d6674-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6674-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6674-110">Permission type</span></span>|<span data-ttu-id="d6674-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6674-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6674-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6674-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d6674-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d6674-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="d6674-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6674-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d6674-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6674-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6674-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6674-116">Not supported.</span></span>|
|<span data-ttu-id="d6674-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6674-117">Application</span></span>||
| <span data-ttu-id="d6674-118">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d6674-118">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="d6674-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6674-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6674-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6674-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="d6674-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6674-121">Request headers</span></span>
|<span data-ttu-id="d6674-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6674-122">Header</span></span>|<span data-ttu-id="d6674-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d6674-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6674-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6674-124">Authorization</span></span>|<span data-ttu-id="d6674-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6674-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6674-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d6674-126">Accept</span></span>|<span data-ttu-id="d6674-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6674-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6674-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6674-128">Request body</span></span>
<span data-ttu-id="d6674-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6674-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d6674-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d6674-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d6674-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6674-131">Property</span></span>|<span data-ttu-id="d6674-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d6674-132">Type</span></span>|<span data-ttu-id="d6674-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d6674-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6674-134">apps</span><span class="sxs-lookup"><span data-stu-id="d6674-134">apps</span></span>|<span data-ttu-id="d6674-135">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d6674-135">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d6674-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6674-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6674-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6674-137">Response</span></span>
<span data-ttu-id="d6674-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6674-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6674-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d6674-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6674-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6674-140">Request</span></span>
<span data-ttu-id="d6674-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6674-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6674-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6674-142">Response</span></span>
<span data-ttu-id="d6674-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6674-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







