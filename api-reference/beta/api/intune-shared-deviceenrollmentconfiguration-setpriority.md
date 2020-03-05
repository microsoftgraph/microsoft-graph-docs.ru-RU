---
title: Действие setPriority
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 637fea767671d2d30a2cb1c94668f3d6e5303f4d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458625"
---
# <a name="setpriority-action"></a><span data-ttu-id="4d6d4-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="4d6d4-103">setPriority action</span></span>

<span data-ttu-id="4d6d4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d6d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d6d4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d6d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d6d4-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d6d4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d6d4-108">Prerequisites</span></span>
<span data-ttu-id="4d6d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d6d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d6d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d6d4-111">Permission type</span></span>|<span data-ttu-id="4d6d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d6d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d6d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d6d4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4d6d4-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4d6d4-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4d6d4-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6d4-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d6d4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d6d4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d6d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-117">Not supported.</span></span>|
|<span data-ttu-id="4d6d4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d6d4-118">Application</span></span>||
| <span data-ttu-id="4d6d4-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4d6d4-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4d6d4-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6d4-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d6d4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d6d4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="4d6d4-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4d6d4-122">Request headers</span></span>
|<span data-ttu-id="4d6d4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d6d4-123">Header</span></span>|<span data-ttu-id="4d6d4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4d6d4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d6d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d6d4-125">Authorization</span></span>|<span data-ttu-id="4d6d4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d6d4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4d6d4-127">Accept</span></span>|<span data-ttu-id="4d6d4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4d6d4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d6d4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d6d4-129">Request body</span></span>
<span data-ttu-id="4d6d4-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d6d4-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d6d4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d6d4-132">Property</span></span>|<span data-ttu-id="4d6d4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4d6d4-133">Type</span></span>|<span data-ttu-id="4d6d4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4d6d4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d6d4-135">priority</span><span class="sxs-lookup"><span data-stu-id="4d6d4-135">priority</span></span>|<span data-ttu-id="4d6d4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6d4-136">Int32</span></span>|<span data-ttu-id="4d6d4-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d6d4-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d6d4-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d6d4-138">Response</span></span>
<span data-ttu-id="4d6d4-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d6d4-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4d6d4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d6d4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d6d4-141">Request</span></span>
<span data-ttu-id="4d6d4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="4d6d4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6d4-143">Response</span></span>
<span data-ttu-id="4d6d4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d6d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








