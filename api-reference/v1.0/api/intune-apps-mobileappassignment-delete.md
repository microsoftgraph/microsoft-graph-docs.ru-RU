---
title: Delete mobileAppAssignment
description: Удаляет объект mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1a0972b3b7e08d3c8e1186cec52ee91cbe7d14d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456419"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="1ca86-103">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="1ca86-103">Delete mobileAppAssignment</span></span>

<span data-ttu-id="1ca86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ca86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ca86-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ca86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca86-106">Удаляет объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ca86-106">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ca86-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca86-107">Prerequisites</span></span>
<span data-ttu-id="1ca86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca86-110">Permission type</span></span>|<span data-ttu-id="1ca86-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca86-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ca86-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ca86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca86-115">Not supported.</span></span>|
|<span data-ttu-id="1ca86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca86-116">Application</span></span>|<span data-ttu-id="1ca86-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ca86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1ca86-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1ca86-119">Request headers</span></span>
|<span data-ttu-id="1ca86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ca86-120">Header</span></span>|<span data-ttu-id="1ca86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1ca86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ca86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ca86-122">Authorization</span></span>|<span data-ttu-id="1ca86-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ca86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1ca86-124">Accept</span></span>|<span data-ttu-id="1ca86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ca86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca86-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ca86-126">Request body</span></span>
<span data-ttu-id="1ca86-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ca86-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ca86-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca86-128">Response</span></span>
<span data-ttu-id="1ca86-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1ca86-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1ca86-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1ca86-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ca86-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca86-131">Request</span></span>
<span data-ttu-id="1ca86-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ca86-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1ca86-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca86-133">Response</span></span>
<span data-ttu-id="1ca86-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ca86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






