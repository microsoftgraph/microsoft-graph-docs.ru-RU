---
title: Delete mobileAppAssignment
description: Удаляет объект mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ce9396f0bb5b6e69cf9d662c1b85cb74599ee25
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761421"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="bb3f4-103">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb3f4-103">Delete mobileAppAssignment</span></span>

> <span data-ttu-id="bb3f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb3f4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb3f4-106">Удаляет объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bb3f4-106">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb3f4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bb3f4-107">Prerequisites</span></span>
<span data-ttu-id="bb3f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb3f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb3f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb3f4-110">Permission type</span></span>|<span data-ttu-id="bb3f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb3f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb3f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb3f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb3f4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb3f4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb3f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb3f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb3f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-115">Not supported.</span></span>|
|<span data-ttu-id="bb3f4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb3f4-116">Application</span></span>|<span data-ttu-id="bb3f4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb3f4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb3f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb3f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bb3f4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb3f4-119">Request headers</span></span>
|<span data-ttu-id="bb3f4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb3f4-120">Header</span></span>|<span data-ttu-id="bb3f4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bb3f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb3f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb3f4-122">Authorization</span></span>|<span data-ttu-id="bb3f4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb3f4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb3f4-124">Accept</span></span>|<span data-ttu-id="bb3f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb3f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb3f4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb3f4-126">Request body</span></span>
<span data-ttu-id="bb3f4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb3f4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb3f4-128">Response</span></span>
<span data-ttu-id="bb3f4-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb3f4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bb3f4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb3f4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb3f4-131">Request</span></span>
<span data-ttu-id="bb3f4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bb3f4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb3f4-133">Response</span></span>
<span data-ttu-id="bb3f4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb3f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




