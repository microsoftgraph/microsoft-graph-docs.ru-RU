---
title: Delete mobileAppCategory
description: Удаляет объект mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62f2297659e50abd435cda985b6bb4a94d5a755b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935864"
---
# <a name="delete-mobileappcategory"></a><span data-ttu-id="7eefa-103">Delete mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="7eefa-103">Delete mobileAppCategory</span></span>

> <span data-ttu-id="7eefa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eefa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7eefa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7eefa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eefa-106">Удаляет объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="7eefa-106">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7eefa-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7eefa-107">Prerequisites</span></span>
<span data-ttu-id="7eefa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eefa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eefa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7eefa-110">Permission type</span></span>|<span data-ttu-id="7eefa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7eefa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eefa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7eefa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7eefa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eefa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7eefa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7eefa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eefa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eefa-115">Not supported.</span></span>|
|<span data-ttu-id="7eefa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7eefa-116">Application</span></span>|<span data-ttu-id="7eefa-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eefa-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eefa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7eefa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="7eefa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7eefa-119">Request headers</span></span>
|<span data-ttu-id="7eefa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7eefa-120">Header</span></span>|<span data-ttu-id="7eefa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7eefa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7eefa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7eefa-122">Authorization</span></span>|<span data-ttu-id="7eefa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eefa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7eefa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7eefa-124">Accept</span></span>|<span data-ttu-id="7eefa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7eefa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eefa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7eefa-126">Request body</span></span>
<span data-ttu-id="7eefa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7eefa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eefa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7eefa-128">Response</span></span>
<span data-ttu-id="7eefa-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7eefa-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7eefa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7eefa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7eefa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7eefa-131">Request</span></span>
<span data-ttu-id="7eefa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7eefa-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="7eefa-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7eefa-133">Response</span></span>
<span data-ttu-id="7eefa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7eefa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





