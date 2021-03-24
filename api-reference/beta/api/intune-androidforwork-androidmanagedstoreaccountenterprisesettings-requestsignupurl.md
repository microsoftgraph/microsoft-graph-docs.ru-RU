---
title: Действие requestSignupUrl
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5aef24c7339401c92686f819dc13433e2ee6228c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141192"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="3eb10-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="3eb10-103">requestSignupUrl action</span></span>

<span data-ttu-id="3eb10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eb10-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eb10-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3eb10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb10-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3eb10-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eb10-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3eb10-108">Prerequisites</span></span>
<span data-ttu-id="3eb10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb10-111">Permission type</span></span>|<span data-ttu-id="3eb10-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eb10-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb10-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eb10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb10-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eb10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb10-116">Not supported.</span></span>|
|<span data-ttu-id="3eb10-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eb10-117">Application</span></span>|<span data-ttu-id="3eb10-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb10-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eb10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="3eb10-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3eb10-120">Request headers</span></span>
|<span data-ttu-id="3eb10-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eb10-121">Header</span></span>|<span data-ttu-id="3eb10-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3eb10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb10-123">Authorization</span></span>|<span data-ttu-id="3eb10-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eb10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb10-125">Accept</span></span>|<span data-ttu-id="3eb10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb10-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eb10-127">Request body</span></span>
<span data-ttu-id="3eb10-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eb10-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3eb10-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3eb10-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3eb10-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eb10-130">Property</span></span>|<span data-ttu-id="3eb10-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb10-131">Type</span></span>|<span data-ttu-id="3eb10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3eb10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb10-133">hostName</span><span class="sxs-lookup"><span data-stu-id="3eb10-133">hostName</span></span>|<span data-ttu-id="3eb10-134">String</span><span class="sxs-lookup"><span data-stu-id="3eb10-134">String</span></span>|<span data-ttu-id="3eb10-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3eb10-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3eb10-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb10-136">Response</span></span>
<span data-ttu-id="3eb10-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3eb10-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb10-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3eb10-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eb10-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eb10-139">Request</span></span>
<span data-ttu-id="3eb10-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eb10-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="3eb10-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb10-141">Response</span></span>
<span data-ttu-id="3eb10-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3eb10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




