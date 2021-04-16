---
title: Удаление targetedManagedAppConfiguration
description: Удаление объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7753f69e040cb2453f8e0fd96078a8d2c7d2bc93
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868129"
---
# <a name="delete-targetedmanagedappconfiguration"></a><span data-ttu-id="73da3-103">Удаление targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="73da3-103">Delete targetedManagedAppConfiguration</span></span>

<span data-ttu-id="73da3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73da3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73da3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73da3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73da3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73da3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73da3-107">Удаление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73da3-107">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73da3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="73da3-108">Prerequisites</span></span>
<span data-ttu-id="73da3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73da3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73da3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73da3-111">Permission type</span></span>|<span data-ttu-id="73da3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73da3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73da3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73da3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73da3-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="73da3-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="73da3-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73da3-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="73da3-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="73da3-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="73da3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73da3-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73da3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73da3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73da3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73da3-119">Not supported.</span></span>|
|<span data-ttu-id="73da3-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="73da3-120">Application</span></span>||
| <span data-ttu-id="73da3-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="73da3-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="73da3-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73da3-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="73da3-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="73da3-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="73da3-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73da3-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73da3-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73da3-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="73da3-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73da3-126">Request headers</span></span>
|<span data-ttu-id="73da3-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73da3-127">Header</span></span>|<span data-ttu-id="73da3-128">Значение</span><span class="sxs-lookup"><span data-stu-id="73da3-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73da3-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73da3-129">Authorization</span></span>|<span data-ttu-id="73da3-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73da3-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73da3-131">Accept</span><span class="sxs-lookup"><span data-stu-id="73da3-131">Accept</span></span>|<span data-ttu-id="73da3-132">application/json</span><span class="sxs-lookup"><span data-stu-id="73da3-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73da3-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73da3-133">Request body</span></span>
<span data-ttu-id="73da3-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73da3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73da3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="73da3-135">Response</span></span>
<span data-ttu-id="73da3-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73da3-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73da3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="73da3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="73da3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="73da3-138">Request</span></span>
<span data-ttu-id="73da3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73da3-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="73da3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="73da3-140">Response</span></span>
<span data-ttu-id="73da3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73da3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







