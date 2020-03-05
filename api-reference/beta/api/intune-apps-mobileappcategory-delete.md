---
title: Delete mobileAppCategory
description: Удаляет объект mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19658ed442f735f92cecc6d3ccfb0fb6dfe5583f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450799"
---
# <a name="delete-mobileappcategory"></a><span data-ttu-id="1bb89-103">Delete mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="1bb89-103">Delete mobileAppCategory</span></span>

<span data-ttu-id="1bb89-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1bb89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bb89-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bb89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bb89-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bb89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb89-107">Удаляет объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="1bb89-107">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bb89-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1bb89-108">Prerequisites</span></span>
<span data-ttu-id="1bb89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bb89-111">Permission type</span></span>|<span data-ttu-id="1bb89-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bb89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb89-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bb89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb89-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb89-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bb89-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bb89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bb89-116">Not supported.</span></span>|
|<span data-ttu-id="1bb89-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bb89-117">Application</span></span>|<span data-ttu-id="1bb89-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb89-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb89-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bb89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="1bb89-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bb89-120">Request headers</span></span>
|<span data-ttu-id="1bb89-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bb89-121">Header</span></span>|<span data-ttu-id="1bb89-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1bb89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bb89-123">Authorization</span></span>|<span data-ttu-id="1bb89-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bb89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bb89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bb89-125">Accept</span></span>|<span data-ttu-id="1bb89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bb89-127">Request body</span></span>
<span data-ttu-id="1bb89-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bb89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bb89-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bb89-129">Response</span></span>
<span data-ttu-id="1bb89-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1bb89-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bb89-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1bb89-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bb89-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bb89-132">Request</span></span>
<span data-ttu-id="1bb89-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bb89-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="1bb89-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bb89-134">Response</span></span>
<span data-ttu-id="1bb89-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bb89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





