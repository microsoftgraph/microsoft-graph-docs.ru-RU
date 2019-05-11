---
title: Действие updateDeviceProfileAssignment
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a578db3df35168a2b16402cd7b2469f2725da924
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909003"
---
# <a name="updatedeviceprofileassignment-action"></a><span data-ttu-id="5de60-103">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5de60-103">updateDeviceProfileAssignment action</span></span>

> <span data-ttu-id="5de60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5de60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5de60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5de60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5de60-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5de60-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5de60-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5de60-107">Prerequisites</span></span>
<span data-ttu-id="5de60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5de60-110">Permission type</span></span>|<span data-ttu-id="5de60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5de60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5de60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5de60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5de60-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de60-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5de60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5de60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5de60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5de60-115">Not supported.</span></span>|
|<span data-ttu-id="5de60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5de60-116">Application</span></span>|<span data-ttu-id="5de60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5de60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5de60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5de60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment
```

## <a name="request-headers"></a><span data-ttu-id="5de60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5de60-119">Request headers</span></span>
|<span data-ttu-id="5de60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5de60-120">Header</span></span>|<span data-ttu-id="5de60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5de60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5de60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5de60-122">Authorization</span></span>|<span data-ttu-id="5de60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5de60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5de60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5de60-124">Accept</span></span>|<span data-ttu-id="5de60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5de60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5de60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5de60-126">Request body</span></span>
<span data-ttu-id="5de60-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5de60-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5de60-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5de60-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5de60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5de60-129">Property</span></span>|<span data-ttu-id="5de60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5de60-130">Type</span></span>|<span data-ttu-id="5de60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5de60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de60-132">Девицеидс</span><span class="sxs-lookup"><span data-stu-id="5de60-132">deviceIds</span></span>|<span data-ttu-id="5de60-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5de60-133">String collection</span></span>|<span data-ttu-id="5de60-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5de60-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5de60-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5de60-135">Response</span></span>
<span data-ttu-id="5de60-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5de60-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5de60-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5de60-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5de60-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de60-138">Request</span></span>
<span data-ttu-id="5de60-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5de60-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5de60-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de60-140">Response</span></span>
<span data-ttu-id="5de60-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5de60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




