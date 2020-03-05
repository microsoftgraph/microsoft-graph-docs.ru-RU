---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаляет объект mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b1e03393901a2b50a99e05d698856032315021f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458359"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="21fdf-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="21fdf-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="21fdf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21fdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21fdf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21fdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21fdf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21fdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21fdf-107">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="21fdf-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21fdf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21fdf-108">Prerequisites</span></span>
<span data-ttu-id="21fdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21fdf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21fdf-111">Permission type</span></span>|<span data-ttu-id="21fdf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21fdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21fdf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21fdf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="21fdf-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="21fdf-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="21fdf-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21fdf-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="21fdf-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="21fdf-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="21fdf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21fdf-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21fdf-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21fdf-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21fdf-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21fdf-119">Not supported.</span></span>|
|<span data-ttu-id="21fdf-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21fdf-120">Application</span></span>||
| <span data-ttu-id="21fdf-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="21fdf-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="21fdf-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21fdf-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="21fdf-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="21fdf-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="21fdf-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21fdf-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21fdf-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21fdf-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="21fdf-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21fdf-126">Request headers</span></span>
|<span data-ttu-id="21fdf-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21fdf-127">Header</span></span>|<span data-ttu-id="21fdf-128">Значение</span><span class="sxs-lookup"><span data-stu-id="21fdf-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21fdf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="21fdf-129">Authorization</span></span>|<span data-ttu-id="21fdf-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21fdf-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21fdf-131">Accept</span><span class="sxs-lookup"><span data-stu-id="21fdf-131">Accept</span></span>|<span data-ttu-id="21fdf-132">application/json</span><span class="sxs-lookup"><span data-stu-id="21fdf-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21fdf-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21fdf-133">Request body</span></span>
<span data-ttu-id="21fdf-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21fdf-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21fdf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="21fdf-135">Response</span></span>
<span data-ttu-id="21fdf-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21fdf-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="21fdf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="21fdf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="21fdf-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="21fdf-138">Request</span></span>
<span data-ttu-id="21fdf-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21fdf-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="21fdf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="21fdf-140">Response</span></span>
<span data-ttu-id="21fdf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21fdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








