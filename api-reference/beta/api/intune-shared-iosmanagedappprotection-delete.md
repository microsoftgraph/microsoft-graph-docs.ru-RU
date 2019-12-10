---
title: Delete iosManagedAppProtection
description: Удаляет объект iosManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 677bbc2ed1fafddfa9083de8a2b42e66f964fe98
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939811"
---
# <a name="delete-iosmanagedappprotection"></a><span data-ttu-id="0ebc6-103">Delete iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="0ebc6-103">Delete iosManagedAppProtection</span></span>

> <span data-ttu-id="0ebc6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ebc6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ebc6-106">Удаляет объект [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ebc6-106">Deletes a [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ebc6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0ebc6-107">Prerequisites</span></span>
<span data-ttu-id="0ebc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ebc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ebc6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ebc6-110">Permission type</span></span>|<span data-ttu-id="0ebc6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ebc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ebc6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ebc6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ebc6-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="0ebc6-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0ebc6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebc6-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="0ebc6-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="0ebc6-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0ebc6-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebc6-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ebc6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ebc6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ebc6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-118">Not supported.</span></span>|
|<span data-ttu-id="0ebc6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ebc6-119">Application</span></span>||
| <span data-ttu-id="0ebc6-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="0ebc6-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0ebc6-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebc6-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="0ebc6-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="0ebc6-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0ebc6-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebc6-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ebc6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ebc6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="0ebc6-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ebc6-125">Request headers</span></span>
|<span data-ttu-id="0ebc6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ebc6-126">Header</span></span>|<span data-ttu-id="0ebc6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="0ebc6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ebc6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ebc6-128">Authorization</span></span>|<span data-ttu-id="0ebc6-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ebc6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="0ebc6-130">Accept</span></span>|<span data-ttu-id="0ebc6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0ebc6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ebc6-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ebc6-132">Request body</span></span>
<span data-ttu-id="0ebc6-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ebc6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ebc6-134">Response</span></span>
<span data-ttu-id="0ebc6-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ebc6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="0ebc6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ebc6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ebc6-137">Request</span></span>
<span data-ttu-id="0ebc6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="0ebc6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ebc6-139">Response</span></span>
<span data-ttu-id="0ebc6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ebc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








