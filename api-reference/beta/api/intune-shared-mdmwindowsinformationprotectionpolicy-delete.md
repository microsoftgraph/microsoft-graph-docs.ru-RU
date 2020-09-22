---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаляет объект mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19ebcaa0e933625435d29024ea6e38fe8dd50ba1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044797"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="887ed-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="887ed-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="887ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="887ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="887ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="887ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="887ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="887ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="887ed-107">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="887ed-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="887ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="887ed-108">Prerequisites</span></span>
<span data-ttu-id="887ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="887ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="887ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="887ed-111">Permission type</span></span>|<span data-ttu-id="887ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="887ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="887ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="887ed-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="887ed-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="887ed-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="887ed-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887ed-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="887ed-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="887ed-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="887ed-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887ed-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="887ed-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="887ed-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="887ed-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="887ed-119">Not supported.</span></span>|
|<span data-ttu-id="887ed-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="887ed-120">Application</span></span>||
| <span data-ttu-id="887ed-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="887ed-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="887ed-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887ed-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="887ed-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="887ed-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="887ed-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887ed-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="887ed-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="887ed-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="887ed-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="887ed-126">Request headers</span></span>
|<span data-ttu-id="887ed-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="887ed-127">Header</span></span>|<span data-ttu-id="887ed-128">Значение</span><span class="sxs-lookup"><span data-stu-id="887ed-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="887ed-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="887ed-129">Authorization</span></span>|<span data-ttu-id="887ed-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="887ed-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="887ed-131">Accept</span><span class="sxs-lookup"><span data-stu-id="887ed-131">Accept</span></span>|<span data-ttu-id="887ed-132">application/json</span><span class="sxs-lookup"><span data-stu-id="887ed-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="887ed-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="887ed-133">Request body</span></span>
<span data-ttu-id="887ed-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="887ed-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="887ed-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="887ed-135">Response</span></span>
<span data-ttu-id="887ed-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="887ed-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="887ed-137">Пример</span><span class="sxs-lookup"><span data-stu-id="887ed-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="887ed-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="887ed-138">Request</span></span>
<span data-ttu-id="887ed-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="887ed-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="887ed-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="887ed-140">Response</span></span>
<span data-ttu-id="887ed-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="887ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









