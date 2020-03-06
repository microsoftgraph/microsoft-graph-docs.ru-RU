---
title: Delete mobileAppContent
description: Удаляет объект mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2a93f13e6bf1e5b741e8735d68d650e7f19723d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515983"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="ada16-103">Delete mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ada16-103">Delete mobileAppContent</span></span>

<span data-ttu-id="ada16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ada16-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ada16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ada16-106">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ada16-106">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ada16-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ada16-107">Prerequisites</span></span>
<span data-ttu-id="ada16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ada16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ada16-110">Permission type</span></span>|<span data-ttu-id="ada16-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ada16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ada16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ada16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ada16-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada16-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ada16-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ada16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ada16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ada16-115">Not supported.</span></span>|
|<span data-ttu-id="ada16-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ada16-116">Application</span></span>|<span data-ttu-id="ada16-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ada16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ada16-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ada16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="ada16-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ada16-119">Request headers</span></span>
|<span data-ttu-id="ada16-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ada16-120">Header</span></span>|<span data-ttu-id="ada16-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ada16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ada16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ada16-122">Authorization</span></span>|<span data-ttu-id="ada16-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ada16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ada16-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ada16-124">Accept</span></span>|<span data-ttu-id="ada16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ada16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ada16-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ada16-126">Request body</span></span>
<span data-ttu-id="ada16-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ada16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ada16-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada16-128">Response</span></span>
<span data-ttu-id="ada16-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ada16-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ada16-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ada16-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ada16-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ada16-131">Request</span></span>
<span data-ttu-id="ada16-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ada16-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="ada16-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada16-133">Response</span></span>
<span data-ttu-id="ada16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ada16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




