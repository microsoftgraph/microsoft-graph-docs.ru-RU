---
title: Действие unbind
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f5e303c1e8ec3bc54c38d264f3274184093ce0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144594"
---
# <a name="unbind-action"></a><span data-ttu-id="16741-103">Действие unbind</span><span class="sxs-lookup"><span data-stu-id="16741-103">unbind action</span></span>

<span data-ttu-id="16741-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16741-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16741-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16741-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16741-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16741-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16741-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="16741-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16741-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16741-108">Prerequisites</span></span>
<span data-ttu-id="16741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16741-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16741-111">Permission type</span></span>|<span data-ttu-id="16741-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16741-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16741-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16741-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16741-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16741-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16741-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16741-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16741-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16741-116">Not supported.</span></span>|
|<span data-ttu-id="16741-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="16741-117">Application</span></span>|<span data-ttu-id="16741-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16741-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16741-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16741-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

## <a name="request-headers"></a><span data-ttu-id="16741-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16741-120">Request headers</span></span>
|<span data-ttu-id="16741-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16741-121">Header</span></span>|<span data-ttu-id="16741-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16741-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16741-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16741-123">Authorization</span></span>|<span data-ttu-id="16741-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16741-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16741-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16741-125">Accept</span></span>|<span data-ttu-id="16741-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16741-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16741-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16741-127">Request body</span></span>
<span data-ttu-id="16741-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16741-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16741-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16741-129">Response</span></span>
<span data-ttu-id="16741-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="16741-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="16741-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16741-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="16741-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16741-132">Request</span></span>
<span data-ttu-id="16741-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16741-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

### <a name="response"></a><span data-ttu-id="16741-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="16741-134">Response</span></span>
<span data-ttu-id="16741-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16741-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




