---
title: Delete mobileAppContent
description: Удаляет объект mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b44aee13184b56ef1dd2d136e6fc3bfb3d1b052e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876379"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="4e48e-103">Delete mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4e48e-103">Delete mobileAppContent</span></span>

> <span data-ttu-id="4e48e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e48e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e48e-105">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4e48e-105">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e48e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4e48e-106">Prerequisites</span></span>
<span data-ttu-id="4e48e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e48e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e48e-109">Permission type</span></span>|<span data-ttu-id="4e48e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e48e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e48e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e48e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e48e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e48e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e48e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e48e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e48e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e48e-114">Not supported.</span></span>|
|<span data-ttu-id="4e48e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e48e-115">Application</span></span>|<span data-ttu-id="4e48e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e48e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e48e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e48e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="4e48e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e48e-118">Request headers</span></span>
|<span data-ttu-id="4e48e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e48e-119">Header</span></span>|<span data-ttu-id="4e48e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4e48e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e48e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e48e-121">Authorization</span></span>|<span data-ttu-id="4e48e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e48e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e48e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4e48e-123">Accept</span></span>|<span data-ttu-id="4e48e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4e48e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e48e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e48e-125">Request body</span></span>
<span data-ttu-id="4e48e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e48e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e48e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e48e-127">Response</span></span>
<span data-ttu-id="4e48e-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e48e-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e48e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4e48e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e48e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e48e-130">Request</span></span>
<span data-ttu-id="4e48e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e48e-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="4e48e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e48e-132">Response</span></span>
<span data-ttu-id="4e48e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e48e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



