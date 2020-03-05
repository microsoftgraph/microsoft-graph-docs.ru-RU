---
title: Удаление androidManagedAppProtection
description: Удаление объекта androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e21d89dc7570c6436b3b9ade4d34f35f0d87191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458975"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="499a4-103">Удаление androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="499a4-103">Delete androidManagedAppProtection</span></span>

<span data-ttu-id="499a4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="499a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="499a4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="499a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="499a4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="499a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="499a4-107">Удаление объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="499a4-107">Deletes a [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="499a4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="499a4-108">Prerequisites</span></span>
<span data-ttu-id="499a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="499a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="499a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="499a4-111">Permission type</span></span>|<span data-ttu-id="499a4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="499a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="499a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="499a4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="499a4-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="499a4-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="499a4-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="499a4-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="499a4-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="499a4-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="499a4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="499a4-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="499a4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="499a4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="499a4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="499a4-119">Not supported.</span></span>|
|<span data-ttu-id="499a4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="499a4-120">Application</span></span>||
| <span data-ttu-id="499a4-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="499a4-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="499a4-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="499a4-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="499a4-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="499a4-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="499a4-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="499a4-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="499a4-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="499a4-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="499a4-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="499a4-126">Request headers</span></span>
|<span data-ttu-id="499a4-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="499a4-127">Header</span></span>|<span data-ttu-id="499a4-128">Значение</span><span class="sxs-lookup"><span data-stu-id="499a4-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="499a4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="499a4-129">Authorization</span></span>|<span data-ttu-id="499a4-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="499a4-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="499a4-131">Accept</span><span class="sxs-lookup"><span data-stu-id="499a4-131">Accept</span></span>|<span data-ttu-id="499a4-132">application/json</span><span class="sxs-lookup"><span data-stu-id="499a4-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="499a4-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="499a4-133">Request body</span></span>
<span data-ttu-id="499a4-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="499a4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="499a4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="499a4-135">Response</span></span>
<span data-ttu-id="499a4-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="499a4-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="499a4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="499a4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="499a4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="499a4-138">Request</span></span>
<span data-ttu-id="499a4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="499a4-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="499a4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="499a4-140">Response</span></span>
<span data-ttu-id="499a4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="499a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








