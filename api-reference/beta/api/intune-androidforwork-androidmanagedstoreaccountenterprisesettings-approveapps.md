---
title: действие approveApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba0e5ad261c1fe4596218d48080a8a9331258655
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141206"
---
# <a name="approveapps-action"></a><span data-ttu-id="74e2c-103">действие approveApps</span><span class="sxs-lookup"><span data-stu-id="74e2c-103">approveApps action</span></span>

<span data-ttu-id="74e2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74e2c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74e2c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74e2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74e2c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="74e2c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74e2c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74e2c-108">Prerequisites</span></span>
<span data-ttu-id="74e2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e2c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74e2c-111">Permission type</span></span>|<span data-ttu-id="74e2c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74e2c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e2c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74e2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74e2c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e2c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74e2c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74e2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e2c-116">Not supported.</span></span>|
|<span data-ttu-id="74e2c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="74e2c-117">Application</span></span>|<span data-ttu-id="74e2c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e2c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e2c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74e2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps
```

## <a name="request-headers"></a><span data-ttu-id="74e2c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74e2c-120">Request headers</span></span>
|<span data-ttu-id="74e2c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74e2c-121">Header</span></span>|<span data-ttu-id="74e2c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74e2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e2c-123">Authorization</span></span>|<span data-ttu-id="74e2c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74e2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74e2c-125">Accept</span></span>|<span data-ttu-id="74e2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74e2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e2c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74e2c-127">Request body</span></span>
<span data-ttu-id="74e2c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74e2c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="74e2c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="74e2c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="74e2c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74e2c-130">Property</span></span>|<span data-ttu-id="74e2c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74e2c-131">Type</span></span>|<span data-ttu-id="74e2c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74e2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e2c-133">packageIds</span><span class="sxs-lookup"><span data-stu-id="74e2c-133">packageIds</span></span>|<span data-ttu-id="74e2c-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74e2c-134">String collection</span></span>|<span data-ttu-id="74e2c-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="74e2c-135">Not yet documented</span></span>|
|<span data-ttu-id="74e2c-136">approveAllPermissions</span><span class="sxs-lookup"><span data-stu-id="74e2c-136">approveAllPermissions</span></span>|<span data-ttu-id="74e2c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="74e2c-137">Boolean</span></span>|<span data-ttu-id="74e2c-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="74e2c-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="74e2c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="74e2c-139">Response</span></span>
<span data-ttu-id="74e2c-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74e2c-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74e2c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="74e2c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e2c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e2c-142">Request</span></span>
<span data-ttu-id="74e2c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74e2c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps

Content-type: application/json
Content-length: 87

{
  "packageIds": [
    "Package Ids value"
  ],
  "approveAllPermissions": true
}
```

### <a name="response"></a><span data-ttu-id="74e2c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e2c-144">Response</span></span>
<span data-ttu-id="74e2c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74e2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




