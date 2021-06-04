---
title: Создание объекта mobileAppCategory
description: Создание объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fbbe320ddcdffa54b6fcccece6c6328edf131d3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754107"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="d515b-103">Создание объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="d515b-103">Create mobileAppCategory</span></span>

<span data-ttu-id="d515b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d515b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d515b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d515b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d515b-106">Создание объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d515b-106">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d515b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d515b-107">Prerequisites</span></span>
<span data-ttu-id="d515b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d515b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d515b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d515b-110">Permission type</span></span>|<span data-ttu-id="d515b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d515b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d515b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d515b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d515b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d515b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d515b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d515b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d515b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d515b-115">Not supported.</span></span>|
|<span data-ttu-id="d515b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d515b-116">Application</span></span>|<span data-ttu-id="d515b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d515b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d515b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d515b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="d515b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d515b-119">Request headers</span></span>
|<span data-ttu-id="d515b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d515b-120">Header</span></span>|<span data-ttu-id="d515b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d515b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d515b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d515b-122">Authorization</span></span>|<span data-ttu-id="d515b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d515b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d515b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d515b-124">Accept</span></span>|<span data-ttu-id="d515b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d515b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d515b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d515b-126">Request body</span></span>
<span data-ttu-id="d515b-127">В тексте запроса добавьте представление объекта mobileAppCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d515b-127">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="d515b-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="d515b-128">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="d515b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d515b-129">Property</span></span>|<span data-ttu-id="d515b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d515b-130">Type</span></span>|<span data-ttu-id="d515b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d515b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d515b-132">id</span><span class="sxs-lookup"><span data-stu-id="d515b-132">id</span></span>|<span data-ttu-id="d515b-133">String</span><span class="sxs-lookup"><span data-stu-id="d515b-133">String</span></span>|<span data-ttu-id="d515b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d515b-134">The key of the entity.</span></span>|
|<span data-ttu-id="d515b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d515b-135">displayName</span></span>|<span data-ttu-id="d515b-136">String</span><span class="sxs-lookup"><span data-stu-id="d515b-136">String</span></span>|<span data-ttu-id="d515b-137">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="d515b-137">The name of the app category.</span></span>|
|<span data-ttu-id="d515b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d515b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="d515b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d515b-139">DateTimeOffset</span></span>|<span data-ttu-id="d515b-140">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="d515b-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d515b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d515b-141">Response</span></span>
<span data-ttu-id="d515b-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d515b-142">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d515b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d515b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d515b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d515b-144">Request</span></span>
<span data-ttu-id="d515b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d515b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d515b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d515b-146">Response</span></span>
<span data-ttu-id="d515b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d515b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




