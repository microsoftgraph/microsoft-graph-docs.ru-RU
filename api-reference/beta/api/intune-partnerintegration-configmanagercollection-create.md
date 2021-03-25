---
title: Создание configManagerCollection
description: Создайте новый объект configManagerCollection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a7fc439408d357d2463fd14c0a8c738e403148a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158754"
---
# <a name="create-configmanagercollection"></a><span data-ttu-id="00f26-103">Создание configManagerCollection</span><span class="sxs-lookup"><span data-stu-id="00f26-103">Create configManagerCollection</span></span>

<span data-ttu-id="00f26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00f26-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00f26-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00f26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00f26-107">Создайте новый [объект configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)</span><span class="sxs-lookup"><span data-stu-id="00f26-107">Create a new [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00f26-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00f26-108">Prerequisites</span></span>
<span data-ttu-id="00f26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f26-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f26-111">Permission type</span></span>|<span data-ttu-id="00f26-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f26-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00f26-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00f26-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f26-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00f26-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00f26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f26-116">Not supported.</span></span>|
|<span data-ttu-id="00f26-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="00f26-117">Application</span></span>|<span data-ttu-id="00f26-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f26-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00f26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="00f26-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00f26-120">Request headers</span></span>
|<span data-ttu-id="00f26-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00f26-121">Header</span></span>|<span data-ttu-id="00f26-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00f26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00f26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00f26-123">Authorization</span></span>|<span data-ttu-id="00f26-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00f26-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00f26-125">Accept</span></span>|<span data-ttu-id="00f26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00f26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00f26-127">Request body</span></span>
<span data-ttu-id="00f26-128">В теле запроса поставляем представление JSON для объекта configManagerCollection.</span><span class="sxs-lookup"><span data-stu-id="00f26-128">In the request body, supply a JSON representation for the configManagerCollection object.</span></span>

<span data-ttu-id="00f26-129">В следующей таблице показаны свойства, необходимые при создании configManagerCollection.</span><span class="sxs-lookup"><span data-stu-id="00f26-129">The following table shows the properties that are required when you create the configManagerCollection.</span></span>

|<span data-ttu-id="00f26-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00f26-130">Property</span></span>|<span data-ttu-id="00f26-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00f26-131">Type</span></span>|<span data-ttu-id="00f26-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00f26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00f26-133">id</span><span class="sxs-lookup"><span data-stu-id="00f26-133">id</span></span>|<span data-ttu-id="00f26-134">Строка</span><span class="sxs-lookup"><span data-stu-id="00f26-134">String</span></span>|<span data-ttu-id="00f26-135">Ключ для коллекции ConfigManager.</span><span class="sxs-lookup"><span data-stu-id="00f26-135">The key for the ConfigManager Collection.</span></span>|
|<span data-ttu-id="00f26-136">displayName</span><span class="sxs-lookup"><span data-stu-id="00f26-136">displayName</span></span>|<span data-ttu-id="00f26-137">Строка</span><span class="sxs-lookup"><span data-stu-id="00f26-137">String</span></span>|<span data-ttu-id="00f26-138">The DisplayName.</span><span class="sxs-lookup"><span data-stu-id="00f26-138">The DisplayName.</span></span>|
|<span data-ttu-id="00f26-139">collectionIdentifier</span><span class="sxs-lookup"><span data-stu-id="00f26-139">collectionIdentifier</span></span>|<span data-ttu-id="00f26-140">Строка</span><span class="sxs-lookup"><span data-stu-id="00f26-140">String</span></span>|<span data-ttu-id="00f26-141">Идентификатор коллекции в SCCM.</span><span class="sxs-lookup"><span data-stu-id="00f26-141">The collection identifier in SCCM.</span></span>|
|<span data-ttu-id="00f26-142">hierarchyName</span><span class="sxs-lookup"><span data-stu-id="00f26-142">hierarchyName</span></span>|<span data-ttu-id="00f26-143">Строка</span><span class="sxs-lookup"><span data-stu-id="00f26-143">String</span></span>|<span data-ttu-id="00f26-144">Имя иерархии.</span><span class="sxs-lookup"><span data-stu-id="00f26-144">The HierarchyName.</span></span>|
|<span data-ttu-id="00f26-145">hierarchyIdentifier</span><span class="sxs-lookup"><span data-stu-id="00f26-145">hierarchyIdentifier</span></span>|<span data-ttu-id="00f26-146">Строка</span><span class="sxs-lookup"><span data-stu-id="00f26-146">String</span></span>|<span data-ttu-id="00f26-147">Идентификатор иерархии.</span><span class="sxs-lookup"><span data-stu-id="00f26-147">The Hierarchy Identifier.</span></span>|
|<span data-ttu-id="00f26-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00f26-148">createdDateTime</span></span>|<span data-ttu-id="00f26-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00f26-149">DateTimeOffset</span></span>|<span data-ttu-id="00f26-150">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="00f26-150">The created date.</span></span>|
|<span data-ttu-id="00f26-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00f26-151">lastModifiedDateTime</span></span>|<span data-ttu-id="00f26-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00f26-152">DateTimeOffset</span></span>|<span data-ttu-id="00f26-153">Дата последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="00f26-153">The last modified date.</span></span>|



## <a name="response"></a><span data-ttu-id="00f26-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f26-154">Response</span></span>
<span data-ttu-id="00f26-155">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="00f26-155">If successful, this method returns a `201 Created` response code and a [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00f26-156">Пример</span><span class="sxs-lookup"><span data-stu-id="00f26-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="00f26-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f26-157">Request</span></span>
<span data-ttu-id="00f26-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f26-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value"
}
```

### <a name="response"></a><span data-ttu-id="00f26-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f26-159">Response</span></span>
<span data-ttu-id="00f26-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00f26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 435

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




