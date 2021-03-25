---
title: Действие setPriority
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61651d6517c0ba06e47b214d6afb7f80d8e54007
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157675"
---
# <a name="setpriority-action"></a><span data-ttu-id="457df-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="457df-103">setPriority action</span></span>

<span data-ttu-id="457df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="457df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="457df-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="457df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="457df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="457df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="457df-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="457df-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="457df-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="457df-108">Prerequisites</span></span>
<span data-ttu-id="457df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="457df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="457df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="457df-111">Permission type</span></span>|<span data-ttu-id="457df-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="457df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457df-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="457df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="457df-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457df-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="457df-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="457df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="457df-116">Not supported.</span></span>|
|<span data-ttu-id="457df-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="457df-117">Application</span></span>|<span data-ttu-id="457df-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457df-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="457df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="457df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="457df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="457df-120">Request headers</span></span>
|<span data-ttu-id="457df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="457df-121">Header</span></span>|<span data-ttu-id="457df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="457df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="457df-123">Authorization</span></span>|<span data-ttu-id="457df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="457df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="457df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="457df-125">Accept</span></span>|<span data-ttu-id="457df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="457df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="457df-127">Request body</span></span>
<span data-ttu-id="457df-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="457df-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="457df-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="457df-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="457df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="457df-130">Property</span></span>|<span data-ttu-id="457df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="457df-131">Type</span></span>|<span data-ttu-id="457df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="457df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457df-133">priority</span><span class="sxs-lookup"><span data-stu-id="457df-133">priority</span></span>|<span data-ttu-id="457df-134">Int32</span><span class="sxs-lookup"><span data-stu-id="457df-134">Int32</span></span>|<span data-ttu-id="457df-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="457df-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="457df-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="457df-136">Response</span></span>
<span data-ttu-id="457df-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="457df-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="457df-138">Пример</span><span class="sxs-lookup"><span data-stu-id="457df-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="457df-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="457df-139">Request</span></span>
<span data-ttu-id="457df-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="457df-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="457df-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="457df-141">Response</span></span>
<span data-ttu-id="457df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="457df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




