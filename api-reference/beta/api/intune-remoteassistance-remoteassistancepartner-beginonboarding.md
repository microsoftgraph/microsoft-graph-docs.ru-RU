---
title: Действие beginOnboarding
description: Запрос на запуск бортового.  Должна быть соединая с соответствующими сведениями учетной записи TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4ffc6dc5ded86e7007c3a3b87fdd2007c792eab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134468"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="be37a-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="be37a-104">beginOnboarding action</span></span>

<span data-ttu-id="be37a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be37a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be37a-106">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be37a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be37a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be37a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be37a-108">Запрос на запуск бортового.</span><span class="sxs-lookup"><span data-stu-id="be37a-108">A request to start onboarding.</span></span>  <span data-ttu-id="be37a-109">Должна быть соединая с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="be37a-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be37a-110">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be37a-110">Prerequisites</span></span>
<span data-ttu-id="be37a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be37a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be37a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be37a-113">Permission type</span></span>|<span data-ttu-id="be37a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be37a-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be37a-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be37a-115">Delegated (work or school account)</span></span>|<span data-ttu-id="be37a-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be37a-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be37a-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be37a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be37a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be37a-118">Not supported.</span></span>|
|<span data-ttu-id="be37a-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="be37a-119">Application</span></span>|<span data-ttu-id="be37a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be37a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be37a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be37a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="be37a-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be37a-122">Request headers</span></span>
|<span data-ttu-id="be37a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be37a-123">Header</span></span>|<span data-ttu-id="be37a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="be37a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be37a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be37a-125">Authorization</span></span>|<span data-ttu-id="be37a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be37a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be37a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="be37a-127">Accept</span></span>|<span data-ttu-id="be37a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be37a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be37a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be37a-129">Request body</span></span>
<span data-ttu-id="be37a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be37a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be37a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="be37a-131">Response</span></span>
<span data-ttu-id="be37a-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be37a-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be37a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="be37a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="be37a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="be37a-134">Request</span></span>
<span data-ttu-id="be37a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be37a-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="be37a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="be37a-136">Response</span></span>
<span data-ttu-id="be37a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be37a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




