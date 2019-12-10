---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаляет объект mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76684309684f762db8c050f479d982ac00d3b917
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939762"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="ad423-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="ad423-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="ad423-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad423-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad423-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad423-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad423-106">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad423-106">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad423-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad423-107">Prerequisites</span></span>
<span data-ttu-id="ad423-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad423-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad423-110">Permission type</span></span>|<span data-ttu-id="ad423-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad423-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad423-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad423-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ad423-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ad423-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ad423-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad423-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ad423-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ad423-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ad423-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad423-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad423-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad423-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad423-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad423-118">Not supported.</span></span>|
|<span data-ttu-id="ad423-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad423-119">Application</span></span>||
| <span data-ttu-id="ad423-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ad423-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ad423-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad423-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ad423-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ad423-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ad423-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad423-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad423-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad423-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ad423-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad423-125">Request headers</span></span>
|<span data-ttu-id="ad423-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad423-126">Header</span></span>|<span data-ttu-id="ad423-127">Значение</span><span class="sxs-lookup"><span data-stu-id="ad423-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad423-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad423-128">Authorization</span></span>|<span data-ttu-id="ad423-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad423-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad423-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ad423-130">Accept</span></span>|<span data-ttu-id="ad423-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ad423-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad423-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad423-132">Request body</span></span>
<span data-ttu-id="ad423-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad423-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad423-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad423-134">Response</span></span>
<span data-ttu-id="ad423-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad423-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad423-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ad423-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad423-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad423-137">Request</span></span>
<span data-ttu-id="ad423-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad423-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="ad423-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad423-139">Response</span></span>
<span data-ttu-id="ad423-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad423-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








