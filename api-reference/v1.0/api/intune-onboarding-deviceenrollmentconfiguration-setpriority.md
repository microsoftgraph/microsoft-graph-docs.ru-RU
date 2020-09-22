---
title: Действие setPriority
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9a18689ddf05db06e7b6ad390363457305e978e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057383"
---
# <a name="setpriority-action"></a><span data-ttu-id="5c3c0-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="5c3c0-103">setPriority action</span></span>

<span data-ttu-id="5c3c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c3c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c3c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3c0-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c3c0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c3c0-107">Prerequisites</span></span>
<span data-ttu-id="5c3c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c3c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c3c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c3c0-110">Permission type</span></span>|<span data-ttu-id="5c3c0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c3c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c3c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c3c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c3c0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c3c0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c3c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c3c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c3c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-115">Not supported.</span></span>|
|<span data-ttu-id="5c3c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c3c0-116">Application</span></span>|<span data-ttu-id="5c3c0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c3c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c3c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="5c3c0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c3c0-119">Request headers</span></span>
|<span data-ttu-id="5c3c0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c3c0-120">Header</span></span>|<span data-ttu-id="5c3c0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c3c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c3c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c3c0-122">Authorization</span></span>|<span data-ttu-id="5c3c0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c3c0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c3c0-124">Accept</span></span>|<span data-ttu-id="5c3c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c3c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c3c0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c3c0-126">Request body</span></span>
<span data-ttu-id="5c3c0-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5c3c0-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5c3c0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c3c0-129">Property</span></span>|<span data-ttu-id="5c3c0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c3c0-130">Type</span></span>|<span data-ttu-id="5c3c0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c3c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c3c0-132">priority</span><span class="sxs-lookup"><span data-stu-id="5c3c0-132">priority</span></span>|<span data-ttu-id="5c3c0-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3c0-133">Int32</span></span>|<span data-ttu-id="5c3c0-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5c3c0-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c3c0-135">Response</span></span>
<span data-ttu-id="5c3c0-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c3c0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5c3c0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c3c0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c3c0-138">Request</span></span>
<span data-ttu-id="5c3c0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="5c3c0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c3c0-140">Response</span></span>
<span data-ttu-id="5c3c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c3c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









