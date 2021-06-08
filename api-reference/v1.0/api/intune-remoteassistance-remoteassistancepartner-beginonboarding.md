---
title: Действие beginOnboarding
description: Запрос на запуск бортового.  Должна быть соединая с соответствующими сведениями учетной записи TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc4285513e9ea847bee5014aeab6e62afd8d6f17
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759039"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="074ba-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="074ba-104">beginOnboarding action</span></span>

<span data-ttu-id="074ba-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="074ba-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="074ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="074ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="074ba-107">Запрос на запуск бортового.</span><span class="sxs-lookup"><span data-stu-id="074ba-107">A request to start onboarding.</span></span>  <span data-ttu-id="074ba-108">Должна быть соединая с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="074ba-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="074ba-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="074ba-109">Prerequisites</span></span>
<span data-ttu-id="074ba-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="074ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="074ba-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="074ba-112">Permission type</span></span>|<span data-ttu-id="074ba-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="074ba-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="074ba-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="074ba-114">Delegated (work or school account)</span></span>|<span data-ttu-id="074ba-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="074ba-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="074ba-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="074ba-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="074ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="074ba-117">Not supported.</span></span>|
|<span data-ttu-id="074ba-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="074ba-118">Application</span></span>|<span data-ttu-id="074ba-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="074ba-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="074ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="074ba-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="074ba-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="074ba-121">Request headers</span></span>
|<span data-ttu-id="074ba-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="074ba-122">Header</span></span>|<span data-ttu-id="074ba-123">Значение</span><span class="sxs-lookup"><span data-stu-id="074ba-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="074ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="074ba-124">Authorization</span></span>|<span data-ttu-id="074ba-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="074ba-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="074ba-126">Accept</span><span class="sxs-lookup"><span data-stu-id="074ba-126">Accept</span></span>|<span data-ttu-id="074ba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="074ba-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="074ba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="074ba-128">Request body</span></span>
<span data-ttu-id="074ba-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="074ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="074ba-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="074ba-130">Response</span></span>
<span data-ttu-id="074ba-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="074ba-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="074ba-132">Пример</span><span class="sxs-lookup"><span data-stu-id="074ba-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="074ba-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="074ba-133">Request</span></span>
<span data-ttu-id="074ba-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="074ba-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="074ba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="074ba-135">Response</span></span>
<span data-ttu-id="074ba-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="074ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




