---
title: Удаление объекта managedMobileApp
description: Удаляет объект managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b810aa841bd1c5a9de5186d3046259d912b75820
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463274"
---
# <a name="delete-managedmobileapp"></a><span data-ttu-id="7d046-103">Удаление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="7d046-103">Delete managedMobileApp</span></span>

<span data-ttu-id="7d046-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d046-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d046-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d046-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d046-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d046-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d046-107">Удаляет объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d046-107">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d046-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d046-108">Prerequisites</span></span>
<span data-ttu-id="7d046-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d046-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d046-111">Permission type</span></span>|<span data-ttu-id="7d046-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d046-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d046-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d046-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d046-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d046-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d046-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d046-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d046-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d046-116">Not supported.</span></span>|
|<span data-ttu-id="7d046-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d046-117">Application</span></span>|<span data-ttu-id="7d046-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d046-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d046-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d046-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7d046-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d046-120">Request headers</span></span>
|<span data-ttu-id="7d046-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d046-121">Header</span></span>|<span data-ttu-id="7d046-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d046-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d046-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d046-123">Authorization</span></span>|<span data-ttu-id="7d046-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d046-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d046-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d046-125">Accept</span></span>|<span data-ttu-id="7d046-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d046-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d046-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d046-127">Request body</span></span>
<span data-ttu-id="7d046-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d046-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d046-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d046-129">Response</span></span>
<span data-ttu-id="7d046-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d046-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d046-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d046-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d046-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d046-132">Request</span></span>
<span data-ttu-id="7d046-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d046-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="7d046-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d046-134">Response</span></span>
<span data-ttu-id="7d046-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d046-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





