---
title: Создание объекта mobileAppCategory
description: Создание объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed43265f316e7ec1ef804ba7a121067debf04572
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404583"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="ab01a-103">Создание объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="ab01a-103">Create mobileAppCategory</span></span>

<span data-ttu-id="ab01a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab01a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab01a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab01a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab01a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab01a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab01a-107">Создание объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ab01a-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab01a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab01a-108">Prerequisites</span></span>
<span data-ttu-id="ab01a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab01a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab01a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab01a-111">Permission type</span></span>|<span data-ttu-id="ab01a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab01a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab01a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab01a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab01a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab01a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab01a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab01a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab01a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab01a-116">Not supported.</span></span>|
|<span data-ttu-id="ab01a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ab01a-117">Application</span></span>|<span data-ttu-id="ab01a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab01a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab01a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab01a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="ab01a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab01a-120">Request headers</span></span>
|<span data-ttu-id="ab01a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab01a-121">Header</span></span>|<span data-ttu-id="ab01a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab01a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab01a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab01a-123">Authorization</span></span>|<span data-ttu-id="ab01a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab01a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab01a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab01a-125">Accept</span></span>|<span data-ttu-id="ab01a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab01a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab01a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab01a-127">Request body</span></span>
<span data-ttu-id="ab01a-128">В тексте запроса добавьте представление объекта mobileAppCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab01a-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="ab01a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="ab01a-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="ab01a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab01a-130">Property</span></span>|<span data-ttu-id="ab01a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab01a-131">Type</span></span>|<span data-ttu-id="ab01a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab01a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab01a-133">id</span><span class="sxs-lookup"><span data-stu-id="ab01a-133">id</span></span>|<span data-ttu-id="ab01a-134">String</span><span class="sxs-lookup"><span data-stu-id="ab01a-134">String</span></span>|<span data-ttu-id="ab01a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab01a-135">The key of the entity.</span></span>|
|<span data-ttu-id="ab01a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ab01a-136">displayName</span></span>|<span data-ttu-id="ab01a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ab01a-137">String</span></span>|<span data-ttu-id="ab01a-138">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="ab01a-138">The name of the app category.</span></span>|
|<span data-ttu-id="ab01a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab01a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ab01a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab01a-140">DateTimeOffset</span></span>|<span data-ttu-id="ab01a-141">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="ab01a-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ab01a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab01a-142">Response</span></span>
<span data-ttu-id="ab01a-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab01a-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab01a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ab01a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab01a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab01a-145">Request</span></span>
<span data-ttu-id="ab01a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab01a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ab01a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab01a-147">Response</span></span>
<span data-ttu-id="ab01a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab01a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



