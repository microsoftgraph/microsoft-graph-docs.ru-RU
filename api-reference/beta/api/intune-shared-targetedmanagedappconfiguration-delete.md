---
title: Удаление targetedManagedAppConfiguration
description: Удаление объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: facef4fe97a71d83d18bf357baa04e7473c82453
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537897"
---
# <a name="delete-targetedmanagedappconfiguration"></a><span data-ttu-id="ea5a0-103">Удаление targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea5a0-103">Delete targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="ea5a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea5a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea5a0-106">Удаление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea5a0-106">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea5a0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea5a0-107">Prerequisites</span></span>
<span data-ttu-id="ea5a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea5a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea5a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea5a0-110">Permission type</span></span>|<span data-ttu-id="ea5a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea5a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea5a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea5a0-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea5a0-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ea5a0-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ea5a0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5a0-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ea5a0-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ea5a0-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="ea5a0-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5a0-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea5a0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea5a0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea5a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-118">Not supported.</span></span>|
|<span data-ttu-id="ea5a0-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea5a0-119">Application</span></span>||
| <span data-ttu-id="ea5a0-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ea5a0-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ea5a0-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5a0-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ea5a0-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ea5a0-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="ea5a0-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5a0-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea5a0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea5a0-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea5a0-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea5a0-125">Request headers</span></span>
|<span data-ttu-id="ea5a0-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea5a0-126">Header</span></span>|<span data-ttu-id="ea5a0-127">Значение</span><span class="sxs-lookup"><span data-stu-id="ea5a0-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea5a0-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea5a0-128">Authorization</span></span>|<span data-ttu-id="ea5a0-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea5a0-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ea5a0-130">Accept</span></span>|<span data-ttu-id="ea5a0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ea5a0-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea5a0-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea5a0-132">Request body</span></span>
<span data-ttu-id="ea5a0-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea5a0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5a0-134">Response</span></span>
<span data-ttu-id="ea5a0-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea5a0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ea5a0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea5a0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea5a0-137">Request</span></span>
<span data-ttu-id="ea5a0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ea5a0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5a0-139">Response</span></span>
<span data-ttu-id="ea5a0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea5a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






