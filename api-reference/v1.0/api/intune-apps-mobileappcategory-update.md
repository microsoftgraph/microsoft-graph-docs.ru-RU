---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5175886ecb5bd414691050f5fa3cb9cc2ba571a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754099"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="7a325-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="7a325-103">Update mobileAppCategory</span></span>

<span data-ttu-id="7a325-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a325-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a325-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a325-106">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="7a325-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a325-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a325-107">Prerequisites</span></span>
<span data-ttu-id="7a325-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a325-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a325-110">Permission type</span></span>|<span data-ttu-id="7a325-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a325-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a325-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a325-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a325-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a325-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a325-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a325-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a325-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a325-115">Not supported.</span></span>|
|<span data-ttu-id="7a325-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7a325-116">Application</span></span>|<span data-ttu-id="7a325-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a325-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a325-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a325-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="7a325-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a325-119">Request headers</span></span>
|<span data-ttu-id="7a325-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a325-120">Header</span></span>|<span data-ttu-id="7a325-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7a325-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a325-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a325-122">Authorization</span></span>|<span data-ttu-id="7a325-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a325-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a325-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7a325-124">Accept</span></span>|<span data-ttu-id="7a325-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a325-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a325-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a325-126">Request body</span></span>
<span data-ttu-id="7a325-127">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a325-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="7a325-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="7a325-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="7a325-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a325-129">Property</span></span>|<span data-ttu-id="7a325-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7a325-130">Type</span></span>|<span data-ttu-id="7a325-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7a325-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a325-132">id</span><span class="sxs-lookup"><span data-stu-id="7a325-132">id</span></span>|<span data-ttu-id="7a325-133">String</span><span class="sxs-lookup"><span data-stu-id="7a325-133">String</span></span>|<span data-ttu-id="7a325-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a325-134">The key of the entity.</span></span>|
|<span data-ttu-id="7a325-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7a325-135">displayName</span></span>|<span data-ttu-id="7a325-136">String</span><span class="sxs-lookup"><span data-stu-id="7a325-136">String</span></span>|<span data-ttu-id="7a325-137">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="7a325-137">The name of the app category.</span></span>|
|<span data-ttu-id="7a325-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a325-138">lastModifiedDateTime</span></span>|<span data-ttu-id="7a325-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a325-139">DateTimeOffset</span></span>|<span data-ttu-id="7a325-140">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="7a325-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="7a325-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a325-141">Response</span></span>
<span data-ttu-id="7a325-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a325-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a325-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7a325-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a325-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a325-144">Request</span></span>
<span data-ttu-id="7a325-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a325-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="7a325-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a325-146">Response</span></span>
<span data-ttu-id="7a325-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a325-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




