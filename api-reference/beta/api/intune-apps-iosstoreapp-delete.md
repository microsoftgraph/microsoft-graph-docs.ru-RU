---
title: Удаление объекта iosStoreApp
description: Удаляет объект iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1fb2d7d7d088e7076648dfb482a1fa0d7f7dc1a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394658"
---
# <a name="delete-iosstoreapp"></a><span data-ttu-id="98bce-103">Удаление объекта iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="98bce-103">Delete iosStoreApp</span></span>

<span data-ttu-id="98bce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98bce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98bce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98bce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98bce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98bce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98bce-107">Удаляет объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="98bce-107">Deletes a [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98bce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98bce-108">Prerequisites</span></span>
<span data-ttu-id="98bce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98bce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98bce-111">Permission type</span></span>|<span data-ttu-id="98bce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98bce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98bce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98bce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98bce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98bce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98bce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98bce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98bce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98bce-116">Not supported.</span></span>|
|<span data-ttu-id="98bce-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="98bce-117">Application</span></span>|<span data-ttu-id="98bce-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98bce-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98bce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98bce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="98bce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98bce-120">Request headers</span></span>
|<span data-ttu-id="98bce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98bce-121">Header</span></span>|<span data-ttu-id="98bce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98bce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98bce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98bce-123">Authorization</span></span>|<span data-ttu-id="98bce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98bce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98bce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98bce-125">Accept</span></span>|<span data-ttu-id="98bce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98bce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98bce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98bce-127">Request body</span></span>
<span data-ttu-id="98bce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98bce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98bce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="98bce-129">Response</span></span>
<span data-ttu-id="98bce-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98bce-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98bce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98bce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="98bce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98bce-132">Request</span></span>
<span data-ttu-id="98bce-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98bce-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="98bce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98bce-134">Response</span></span>
<span data-ttu-id="98bce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98bce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



