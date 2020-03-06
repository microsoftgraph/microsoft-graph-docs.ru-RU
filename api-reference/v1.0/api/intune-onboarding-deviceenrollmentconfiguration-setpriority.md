---
title: Действие setPriority
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d498bf9364ad68080b50ac2845ba5b241fba4ad0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512701"
---
# <a name="setpriority-action"></a><span data-ttu-id="7a772-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="7a772-103">setPriority action</span></span>

<span data-ttu-id="7a772-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a772-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a772-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a772-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a772-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7a772-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a772-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a772-107">Prerequisites</span></span>
<span data-ttu-id="7a772-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a772-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a772-110">Permission type</span></span>|<span data-ttu-id="7a772-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a772-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a772-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a772-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a772-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a772-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7a772-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a772-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a772-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a772-115">Not supported.</span></span>|
|<span data-ttu-id="7a772-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a772-116">Application</span></span>|<span data-ttu-id="7a772-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a772-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a772-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a772-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="7a772-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a772-119">Request headers</span></span>
|<span data-ttu-id="7a772-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a772-120">Header</span></span>|<span data-ttu-id="7a772-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7a772-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a772-122">Authorization</span></span>|<span data-ttu-id="7a772-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a772-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a772-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7a772-124">Accept</span></span>|<span data-ttu-id="7a772-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a772-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a772-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a772-126">Request body</span></span>
<span data-ttu-id="7a772-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a772-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7a772-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7a772-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7a772-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a772-129">Property</span></span>|<span data-ttu-id="7a772-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7a772-130">Type</span></span>|<span data-ttu-id="7a772-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7a772-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a772-132">priority</span><span class="sxs-lookup"><span data-stu-id="7a772-132">priority</span></span>|<span data-ttu-id="7a772-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7a772-133">Int32</span></span>|<span data-ttu-id="7a772-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7a772-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7a772-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a772-135">Response</span></span>
<span data-ttu-id="7a772-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a772-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a772-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7a772-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a772-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a772-138">Request</span></span>
<span data-ttu-id="7a772-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a772-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="7a772-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a772-140">Response</span></span>
<span data-ttu-id="7a772-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a772-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




