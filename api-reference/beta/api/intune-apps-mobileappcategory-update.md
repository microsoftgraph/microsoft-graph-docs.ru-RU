---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5382379069debbcf6a733dc917a787cdba0ba9d1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935246"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="46467-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="46467-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="46467-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46467-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46467-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46467-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46467-106">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="46467-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46467-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46467-107">Prerequisites</span></span>
<span data-ttu-id="46467-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46467-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46467-110">Permission type</span></span>|<span data-ttu-id="46467-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46467-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46467-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46467-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46467-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46467-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46467-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46467-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46467-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46467-115">Not supported.</span></span>|
|<span data-ttu-id="46467-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46467-116">Application</span></span>|<span data-ttu-id="46467-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46467-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46467-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46467-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="46467-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46467-119">Request headers</span></span>
|<span data-ttu-id="46467-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46467-120">Header</span></span>|<span data-ttu-id="46467-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46467-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46467-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46467-122">Authorization</span></span>|<span data-ttu-id="46467-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46467-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46467-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46467-124">Accept</span></span>|<span data-ttu-id="46467-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46467-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46467-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46467-126">Request body</span></span>
<span data-ttu-id="46467-127">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46467-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="46467-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="46467-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="46467-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46467-129">Property</span></span>|<span data-ttu-id="46467-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46467-130">Type</span></span>|<span data-ttu-id="46467-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46467-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46467-132">id</span><span class="sxs-lookup"><span data-stu-id="46467-132">id</span></span>|<span data-ttu-id="46467-133">String</span><span class="sxs-lookup"><span data-stu-id="46467-133">String</span></span>|<span data-ttu-id="46467-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46467-134">The key of the entity.</span></span>|
|<span data-ttu-id="46467-135">displayName</span><span class="sxs-lookup"><span data-stu-id="46467-135">displayName</span></span>|<span data-ttu-id="46467-136">Строка</span><span class="sxs-lookup"><span data-stu-id="46467-136">String</span></span>|<span data-ttu-id="46467-137">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="46467-137">The name of the app category.</span></span>|
|<span data-ttu-id="46467-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46467-138">lastModifiedDateTime</span></span>|<span data-ttu-id="46467-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46467-139">DateTimeOffset</span></span>|<span data-ttu-id="46467-140">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="46467-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="46467-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="46467-141">Response</span></span>
<span data-ttu-id="46467-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46467-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46467-143">Пример</span><span class="sxs-lookup"><span data-stu-id="46467-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="46467-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="46467-144">Request</span></span>
<span data-ttu-id="46467-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46467-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="46467-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="46467-146">Response</span></span>
<span data-ttu-id="46467-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46467-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




