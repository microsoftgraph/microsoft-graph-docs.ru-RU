---
title: Действие targetApps
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0ddee6a006f406d3dce717f6e0ed6ee07e55de9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781024"
---
# <a name="targetapps-action"></a><span data-ttu-id="f9951-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="f9951-103">targetApps action</span></span>

> <span data-ttu-id="f9951-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9951-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9951-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9951-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9951-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f9951-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9951-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f9951-107">Prerequisites</span></span>
<span data-ttu-id="f9951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9951-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9951-110">Permission type</span></span>|<span data-ttu-id="f9951-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9951-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9951-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9951-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9951-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9951-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9951-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9951-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9951-115">Not supported.</span></span>|
|<span data-ttu-id="f9951-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9951-116">Application</span></span>|<span data-ttu-id="f9951-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9951-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9951-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9951-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="f9951-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9951-119">Request headers</span></span>
|<span data-ttu-id="f9951-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9951-120">Header</span></span>|<span data-ttu-id="f9951-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9951-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9951-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9951-122">Authorization</span></span>|<span data-ttu-id="f9951-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9951-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9951-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9951-124">Accept</span></span>|<span data-ttu-id="f9951-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9951-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9951-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9951-126">Request body</span></span>
<span data-ttu-id="f9951-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9951-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f9951-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f9951-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f9951-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9951-129">Property</span></span>|<span data-ttu-id="f9951-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f9951-130">Type</span></span>|<span data-ttu-id="f9951-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f9951-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9951-132">apps</span><span class="sxs-lookup"><span data-stu-id="f9951-132">apps</span></span>|<span data-ttu-id="f9951-133">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f9951-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="f9951-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f9951-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f9951-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9951-135">Response</span></span>
<span data-ttu-id="f9951-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9951-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9951-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f9951-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9951-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9951-138">Request</span></span>
<span data-ttu-id="f9951-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9951-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9951-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9951-140">Response</span></span>
<span data-ttu-id="f9951-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9951-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





