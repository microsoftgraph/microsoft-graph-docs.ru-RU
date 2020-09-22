---
title: Delete managedAndroidLobApp
description: Удаляет объект managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d2f09d26cf2b3beb4b28afbf1bf601e300bcfa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973108"
---
# <a name="delete-managedandroidlobapp"></a><span data-ttu-id="ed20a-103">Delete managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="ed20a-103">Delete managedAndroidLobApp</span></span>

<span data-ttu-id="ed20a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed20a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed20a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed20a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed20a-106">Удаляет объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed20a-106">Deletes a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed20a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ed20a-107">Prerequisites</span></span>
<span data-ttu-id="ed20a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed20a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed20a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed20a-110">Permission type</span></span>|<span data-ttu-id="ed20a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed20a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed20a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed20a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed20a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed20a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed20a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed20a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed20a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed20a-115">Not supported.</span></span>|
|<span data-ttu-id="ed20a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed20a-116">Application</span></span>|<span data-ttu-id="ed20a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed20a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed20a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed20a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ed20a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ed20a-119">Request headers</span></span>
|<span data-ttu-id="ed20a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed20a-120">Header</span></span>|<span data-ttu-id="ed20a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ed20a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed20a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed20a-122">Authorization</span></span>|<span data-ttu-id="ed20a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed20a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed20a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ed20a-124">Accept</span></span>|<span data-ttu-id="ed20a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed20a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed20a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed20a-126">Request body</span></span>
<span data-ttu-id="ed20a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed20a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed20a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed20a-128">Response</span></span>
<span data-ttu-id="ed20a-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed20a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed20a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ed20a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed20a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed20a-131">Request</span></span>
<span data-ttu-id="ed20a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed20a-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ed20a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed20a-133">Response</span></span>
<span data-ttu-id="ed20a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed20a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









