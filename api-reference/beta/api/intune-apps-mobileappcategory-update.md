---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d19dcdb6c4223df10b657d2e599d7803878a82c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143299"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="01272-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="01272-103">Update mobileAppCategory</span></span>

<span data-ttu-id="01272-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01272-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01272-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01272-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01272-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01272-107">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="01272-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01272-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01272-108">Prerequisites</span></span>
<span data-ttu-id="01272-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01272-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01272-111">Permission type</span></span>|<span data-ttu-id="01272-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01272-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01272-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01272-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01272-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01272-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01272-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01272-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01272-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01272-116">Not supported.</span></span>|
|<span data-ttu-id="01272-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="01272-117">Application</span></span>|<span data-ttu-id="01272-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01272-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01272-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01272-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="01272-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01272-120">Request headers</span></span>
|<span data-ttu-id="01272-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01272-121">Header</span></span>|<span data-ttu-id="01272-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01272-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01272-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01272-123">Authorization</span></span>|<span data-ttu-id="01272-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01272-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01272-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01272-125">Accept</span></span>|<span data-ttu-id="01272-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01272-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01272-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01272-127">Request body</span></span>
<span data-ttu-id="01272-128">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01272-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="01272-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="01272-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="01272-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01272-130">Property</span></span>|<span data-ttu-id="01272-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01272-131">Type</span></span>|<span data-ttu-id="01272-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01272-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01272-133">id</span><span class="sxs-lookup"><span data-stu-id="01272-133">id</span></span>|<span data-ttu-id="01272-134">Строка</span><span class="sxs-lookup"><span data-stu-id="01272-134">String</span></span>|<span data-ttu-id="01272-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01272-135">The key of the entity.</span></span>|
|<span data-ttu-id="01272-136">displayName</span><span class="sxs-lookup"><span data-stu-id="01272-136">displayName</span></span>|<span data-ttu-id="01272-137">Строка</span><span class="sxs-lookup"><span data-stu-id="01272-137">String</span></span>|<span data-ttu-id="01272-138">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="01272-138">The name of the app category.</span></span>|
|<span data-ttu-id="01272-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01272-139">lastModifiedDateTime</span></span>|<span data-ttu-id="01272-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01272-140">DateTimeOffset</span></span>|<span data-ttu-id="01272-141">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="01272-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="01272-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="01272-142">Response</span></span>
<span data-ttu-id="01272-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01272-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01272-144">Пример</span><span class="sxs-lookup"><span data-stu-id="01272-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="01272-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="01272-145">Request</span></span>
<span data-ttu-id="01272-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01272-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="01272-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="01272-147">Response</span></span>
<span data-ttu-id="01272-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01272-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




