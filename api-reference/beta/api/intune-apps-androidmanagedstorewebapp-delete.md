---
title: Удаление Андроидманажедсторевебапп
description: Удаляет объект Андроидманажедсторевебапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b7f902580ca54fbfaa0023d3021cf6dc80a7c9a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253490"
---
# <a name="delete-androidmanagedstorewebapp"></a><span data-ttu-id="a50ac-103">Удаление Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="a50ac-103">Delete androidManagedStoreWebApp</span></span>

<span data-ttu-id="a50ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a50ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a50ac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a50ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a50ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a50ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a50ac-107">Удаляет объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="a50ac-107">Deletes a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a50ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a50ac-108">Prerequisites</span></span>
<span data-ttu-id="a50ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a50ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a50ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a50ac-111">Permission type</span></span>|<span data-ttu-id="a50ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a50ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a50ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a50ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a50ac-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a50ac-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a50ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a50ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a50ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a50ac-116">Not supported.</span></span>|
|<span data-ttu-id="a50ac-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a50ac-117">Application</span></span>|<span data-ttu-id="a50ac-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a50ac-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a50ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a50ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a50ac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a50ac-120">Request headers</span></span>
|<span data-ttu-id="a50ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a50ac-121">Header</span></span>|<span data-ttu-id="a50ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a50ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a50ac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a50ac-123">Authorization</span></span>|<span data-ttu-id="a50ac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a50ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a50ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a50ac-125">Accept</span></span>|<span data-ttu-id="a50ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a50ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a50ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a50ac-127">Request body</span></span>
<span data-ttu-id="a50ac-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a50ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a50ac-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a50ac-129">Response</span></span>
<span data-ttu-id="a50ac-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a50ac-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a50ac-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a50ac-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a50ac-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a50ac-132">Request</span></span>
<span data-ttu-id="a50ac-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a50ac-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a50ac-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a50ac-134">Response</span></span>
<span data-ttu-id="a50ac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a50ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




