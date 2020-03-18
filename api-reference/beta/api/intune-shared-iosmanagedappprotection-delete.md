---
title: Delete iosManagedAppProtection
description: Удаляет объект iosManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 938730f4fbe9b0c95e7753333d1e9499c07b8b44
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800888"
---
# <a name="delete-iosmanagedappprotection"></a><span data-ttu-id="00268-103">Delete iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="00268-103">Delete iosManagedAppProtection</span></span>

> <span data-ttu-id="00268-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00268-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00268-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00268-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00268-106">Удаляет объект [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="00268-106">Deletes a [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00268-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="00268-107">Prerequisites</span></span>
<span data-ttu-id="00268-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00268-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00268-110">Permission type</span></span>|<span data-ttu-id="00268-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00268-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00268-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00268-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="00268-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="00268-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="00268-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00268-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="00268-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="00268-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="00268-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00268-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00268-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00268-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00268-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00268-118">Not supported.</span></span>|
|<span data-ttu-id="00268-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="00268-119">Application</span></span>||
| <span data-ttu-id="00268-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="00268-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="00268-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00268-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="00268-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="00268-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="00268-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00268-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00268-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00268-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="00268-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00268-125">Request headers</span></span>
|<span data-ttu-id="00268-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00268-126">Header</span></span>|<span data-ttu-id="00268-127">Значение</span><span class="sxs-lookup"><span data-stu-id="00268-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00268-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="00268-128">Authorization</span></span>|<span data-ttu-id="00268-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00268-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00268-130">Accept</span><span class="sxs-lookup"><span data-stu-id="00268-130">Accept</span></span>|<span data-ttu-id="00268-131">application/json</span><span class="sxs-lookup"><span data-stu-id="00268-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00268-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00268-132">Request body</span></span>
<span data-ttu-id="00268-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00268-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00268-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="00268-134">Response</span></span>
<span data-ttu-id="00268-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="00268-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="00268-136">Пример</span><span class="sxs-lookup"><span data-stu-id="00268-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="00268-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="00268-137">Request</span></span>
<span data-ttu-id="00268-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00268-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="00268-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="00268-139">Response</span></span>
<span data-ttu-id="00268-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00268-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







