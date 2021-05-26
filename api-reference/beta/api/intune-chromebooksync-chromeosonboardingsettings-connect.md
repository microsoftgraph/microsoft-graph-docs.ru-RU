---
title: подключение действия
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8acaa40e29e76dfd0d71652339664688a0147cf6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665978"
---
# <a name="connect-action"></a><span data-ttu-id="013d5-103">подключение действия</span><span class="sxs-lookup"><span data-stu-id="013d5-103">connect action</span></span>

<span data-ttu-id="013d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="013d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="013d5-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="013d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="013d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="013d5-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="013d5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="013d5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="013d5-108">Prerequisites</span></span>
<span data-ttu-id="013d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="013d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="013d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="013d5-111">Permission type</span></span>|<span data-ttu-id="013d5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="013d5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="013d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="013d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="013d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="013d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="013d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="013d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013d5-116">Not supported.</span></span>|
|<span data-ttu-id="013d5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="013d5-117">Application</span></span>|<span data-ttu-id="013d5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013d5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="013d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="013d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings/connect
```

## <a name="request-headers"></a><span data-ttu-id="013d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="013d5-120">Request headers</span></span>
|<span data-ttu-id="013d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="013d5-121">Header</span></span>|<span data-ttu-id="013d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="013d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="013d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="013d5-123">Authorization</span></span>|<span data-ttu-id="013d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="013d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="013d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="013d5-125">Accept</span></span>|<span data-ttu-id="013d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="013d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="013d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="013d5-127">Request body</span></span>
<span data-ttu-id="013d5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="013d5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="013d5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="013d5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="013d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="013d5-130">Property</span></span>|<span data-ttu-id="013d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="013d5-131">Type</span></span>|<span data-ttu-id="013d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="013d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013d5-133">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="013d5-133">ownerUserPrincipalName</span></span>|<span data-ttu-id="013d5-134">String</span><span class="sxs-lookup"><span data-stu-id="013d5-134">String</span></span>|<span data-ttu-id="013d5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="013d5-135">Not yet documented</span></span>|
|<span data-ttu-id="013d5-136">serviceAccountCredentials</span><span class="sxs-lookup"><span data-stu-id="013d5-136">serviceAccountCredentials</span></span>|<span data-ttu-id="013d5-137">String</span><span class="sxs-lookup"><span data-stu-id="013d5-137">String</span></span>|<span data-ttu-id="013d5-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="013d5-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="013d5-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="013d5-139">Response</span></span>
<span data-ttu-id="013d5-140">В случае успеха это действие возвращает код отклика и `200 OK` [chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="013d5-140">If successful, this action returns a `200 OK` response code and a [chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013d5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="013d5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="013d5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="013d5-142">Request</span></span>
<span data-ttu-id="013d5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="013d5-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/connect

Content-type: application/json
Content-length: 136

{
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "serviceAccountCredentials": "Service Account Credentials value"
}
```

### <a name="response"></a><span data-ttu-id="013d5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="013d5-144">Response</span></span>
<span data-ttu-id="013d5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="013d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 29

{
  "value": "inprogress"
}
```




