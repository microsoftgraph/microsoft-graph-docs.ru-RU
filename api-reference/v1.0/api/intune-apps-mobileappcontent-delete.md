---
title: Delete mobileAppContent
description: Удаляет объект mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1814f416e16e5541083ec17f7c6042486b35cc6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355073"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="5976f-103">Delete mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5976f-103">Delete mobileAppContent</span></span>

> <span data-ttu-id="5976f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5976f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5976f-105">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5976f-105">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5976f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5976f-106">Prerequisites</span></span>
<span data-ttu-id="5976f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5976f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5976f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5976f-109">Permission type</span></span>|<span data-ttu-id="5976f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5976f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5976f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5976f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5976f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5976f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5976f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5976f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5976f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5976f-114">Not supported.</span></span>|
|<span data-ttu-id="5976f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5976f-115">Application</span></span>|<span data-ttu-id="5976f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5976f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5976f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5976f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="5976f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5976f-118">Request headers</span></span>
|<span data-ttu-id="5976f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5976f-119">Header</span></span>|<span data-ttu-id="5976f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5976f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5976f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5976f-121">Authorization</span></span>|<span data-ttu-id="5976f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5976f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5976f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5976f-123">Accept</span></span>|<span data-ttu-id="5976f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5976f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5976f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5976f-125">Request body</span></span>
<span data-ttu-id="5976f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5976f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5976f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5976f-127">Response</span></span>
<span data-ttu-id="5976f-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5976f-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5976f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5976f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5976f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5976f-130">Request</span></span>
<span data-ttu-id="5976f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5976f-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="5976f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5976f-132">Response</span></span>
<span data-ttu-id="5976f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5976f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




