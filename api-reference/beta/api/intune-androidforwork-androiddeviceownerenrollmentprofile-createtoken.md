---
title: Действие createToken
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7881eddad5c351fc7cd703b2c510bee3b42fc474
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990594"
---
# <a name="createtoken-action"></a><span data-ttu-id="0a9d7-103">Действие createToken</span><span class="sxs-lookup"><span data-stu-id="0a9d7-103">createToken action</span></span>

<span data-ttu-id="0a9d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a9d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a9d7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a9d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a9d7-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a9d7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0a9d7-108">Prerequisites</span></span>
<span data-ttu-id="0a9d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a9d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a9d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9d7-111">Permission type</span></span>|<span data-ttu-id="0a9d7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a9d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a9d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a9d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a9d7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a9d7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a9d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a9d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a9d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-116">Not supported.</span></span>|
|<span data-ttu-id="0a9d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a9d7-117">Application</span></span>|<span data-ttu-id="0a9d7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a9d7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a9d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a9d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="0a9d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a9d7-120">Request headers</span></span>
|<span data-ttu-id="0a9d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a9d7-121">Header</span></span>|<span data-ttu-id="0a9d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a9d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a9d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a9d7-123">Authorization</span></span>|<span data-ttu-id="0a9d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a9d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a9d7-125">Accept</span></span>|<span data-ttu-id="0a9d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a9d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a9d7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a9d7-127">Request body</span></span>
<span data-ttu-id="0a9d7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a9d7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a9d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a9d7-130">Property</span></span>|<span data-ttu-id="0a9d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a9d7-131">Type</span></span>|<span data-ttu-id="0a9d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a9d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a9d7-133">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="0a9d7-133">tokenValidityInSeconds</span></span>|<span data-ttu-id="0a9d7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0a9d7-134">Int32</span></span>|<span data-ttu-id="0a9d7-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a9d7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a9d7-136">Response</span></span>
<span data-ttu-id="0a9d7-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a9d7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0a9d7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a9d7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a9d7-139">Request</span></span>
<span data-ttu-id="0a9d7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="0a9d7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a9d7-141">Response</span></span>
<span data-ttu-id="0a9d7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a9d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






