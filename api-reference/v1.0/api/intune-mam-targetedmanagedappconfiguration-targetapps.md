---
title: Действие targetApps
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ed4c005de0b06d3a4c3ed11c984004e7229c7b5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363250"
---
# <a name="targetapps-action"></a><span data-ttu-id="ea9bf-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="ea9bf-103">targetApps action</span></span>

> <span data-ttu-id="ea9bf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea9bf-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea9bf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea9bf-106">Prerequisites</span></span>
<span data-ttu-id="ea9bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea9bf-109">Permission type</span></span>|<span data-ttu-id="ea9bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea9bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea9bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea9bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea9bf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9bf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea9bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea9bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea9bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-114">Not supported.</span></span>|
|<span data-ttu-id="ea9bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea9bf-115">Application</span></span>|<span data-ttu-id="ea9bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea9bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea9bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="ea9bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea9bf-118">Request headers</span></span>
|<span data-ttu-id="ea9bf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea9bf-119">Header</span></span>|<span data-ttu-id="ea9bf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ea9bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea9bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea9bf-121">Authorization</span></span>|<span data-ttu-id="ea9bf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea9bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ea9bf-123">Accept</span></span>|<span data-ttu-id="ea9bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ea9bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea9bf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea9bf-125">Request body</span></span>
<span data-ttu-id="ea9bf-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea9bf-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea9bf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea9bf-128">Property</span></span>|<span data-ttu-id="ea9bf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ea9bf-129">Type</span></span>|<span data-ttu-id="ea9bf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ea9bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea9bf-131">apps</span><span class="sxs-lookup"><span data-stu-id="ea9bf-131">apps</span></span>|<span data-ttu-id="ea9bf-132">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea9bf-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="ea9bf-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea9bf-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea9bf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea9bf-134">Response</span></span>
<span data-ttu-id="ea9bf-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea9bf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ea9bf-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea9bf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea9bf-137">Request</span></span>
<span data-ttu-id="ea9bf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

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

### <a name="response"></a><span data-ttu-id="ea9bf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea9bf-139">Response</span></span>
<span data-ttu-id="ea9bf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea9bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




