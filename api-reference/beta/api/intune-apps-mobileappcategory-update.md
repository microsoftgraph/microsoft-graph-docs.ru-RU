---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4500d70e3bf86dea2fd58dfe2e0dc387cf97c1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960946"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="8d05d-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="8d05d-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="8d05d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d05d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d05d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d05d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d05d-106">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8d05d-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d05d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8d05d-107">Prerequisites</span></span>
<span data-ttu-id="8d05d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d05d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d05d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d05d-110">Permission type</span></span>|<span data-ttu-id="8d05d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d05d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d05d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d05d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d05d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d05d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d05d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d05d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d05d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d05d-115">Not supported.</span></span>|
|<span data-ttu-id="8d05d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d05d-116">Application</span></span>|<span data-ttu-id="8d05d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d05d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d05d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d05d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="8d05d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d05d-119">Request headers</span></span>
|<span data-ttu-id="8d05d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d05d-120">Header</span></span>|<span data-ttu-id="8d05d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d05d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d05d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d05d-122">Authorization</span></span>|<span data-ttu-id="8d05d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d05d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d05d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d05d-124">Accept</span></span>|<span data-ttu-id="8d05d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d05d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d05d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d05d-126">Request body</span></span>
<span data-ttu-id="8d05d-127">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d05d-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="8d05d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8d05d-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="8d05d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d05d-129">Property</span></span>|<span data-ttu-id="8d05d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d05d-130">Type</span></span>|<span data-ttu-id="8d05d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d05d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d05d-132">id</span><span class="sxs-lookup"><span data-stu-id="8d05d-132">id</span></span>|<span data-ttu-id="8d05d-133">String</span><span class="sxs-lookup"><span data-stu-id="8d05d-133">String</span></span>|<span data-ttu-id="8d05d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d05d-134">The key of the entity.</span></span>|
|<span data-ttu-id="8d05d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8d05d-135">displayName</span></span>|<span data-ttu-id="8d05d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8d05d-136">String</span></span>|<span data-ttu-id="8d05d-137">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="8d05d-137">The name of the app category.</span></span>|
|<span data-ttu-id="8d05d-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d05d-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8d05d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d05d-139">DateTimeOffset</span></span>|<span data-ttu-id="8d05d-140">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="8d05d-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8d05d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d05d-141">Response</span></span>
<span data-ttu-id="8d05d-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d05d-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d05d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8d05d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d05d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d05d-144">Request</span></span>
<span data-ttu-id="8d05d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d05d-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="8d05d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d05d-146">Response</span></span>
<span data-ttu-id="8d05d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d05d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





