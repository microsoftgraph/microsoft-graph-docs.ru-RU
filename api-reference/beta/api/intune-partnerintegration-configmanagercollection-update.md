---
title: Обновление Конфигманажерколлектион
description: Обновление свойств объекта Конфигманажерколлектион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4af6fa3f398022f8abe6d611122d8532e994864
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302266"
---
# <a name="update-configmanagercollection"></a><span data-ttu-id="4b961-103">Обновление Конфигманажерколлектион</span><span class="sxs-lookup"><span data-stu-id="4b961-103">Update configManagerCollection</span></span>

<span data-ttu-id="4b961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b961-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b961-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b961-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b961-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b961-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b961-107">Обновление свойств объекта [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .</span><span class="sxs-lookup"><span data-stu-id="4b961-107">Update the properties of a [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b961-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b961-108">Prerequisites</span></span>
<span data-ttu-id="4b961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b961-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b961-111">Permission type</span></span>|<span data-ttu-id="4b961-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b961-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b961-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b961-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b961-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b961-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b961-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b961-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b961-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b961-116">Not supported.</span></span>|
|<span data-ttu-id="4b961-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b961-117">Application</span></span>|<span data-ttu-id="4b961-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b961-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b961-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b961-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configManagerCollections/{configManagerCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="4b961-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b961-120">Request headers</span></span>
|<span data-ttu-id="4b961-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b961-121">Header</span></span>|<span data-ttu-id="4b961-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b961-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b961-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b961-123">Authorization</span></span>|<span data-ttu-id="4b961-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b961-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b961-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b961-125">Accept</span></span>|<span data-ttu-id="4b961-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b961-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b961-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b961-127">Request body</span></span>
<span data-ttu-id="4b961-128">В тексте запроса добавьте представление объекта [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b961-128">In the request body, supply a JSON representation for the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

<span data-ttu-id="4b961-129">В следующей таблице приведены свойства, необходимые при создании [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md).</span><span class="sxs-lookup"><span data-stu-id="4b961-129">The following table shows the properties that are required when you create the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md).</span></span>

|<span data-ttu-id="4b961-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b961-130">Property</span></span>|<span data-ttu-id="4b961-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b961-131">Type</span></span>|<span data-ttu-id="4b961-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b961-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b961-133">id</span><span class="sxs-lookup"><span data-stu-id="4b961-133">id</span></span>|<span data-ttu-id="4b961-134">String</span><span class="sxs-lookup"><span data-stu-id="4b961-134">String</span></span>|<span data-ttu-id="4b961-135">Ключ для коллекции Конфигманажер.</span><span class="sxs-lookup"><span data-stu-id="4b961-135">The key for the ConfigManager Collection.</span></span>|
|<span data-ttu-id="4b961-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b961-136">displayName</span></span>|<span data-ttu-id="4b961-137">String</span><span class="sxs-lookup"><span data-stu-id="4b961-137">String</span></span>|<span data-ttu-id="4b961-138">DisplayName.</span><span class="sxs-lookup"><span data-stu-id="4b961-138">The DisplayName.</span></span>|
|<span data-ttu-id="4b961-139">коллектионидентифиер</span><span class="sxs-lookup"><span data-stu-id="4b961-139">collectionIdentifier</span></span>|<span data-ttu-id="4b961-140">String</span><span class="sxs-lookup"><span data-stu-id="4b961-140">String</span></span>|<span data-ttu-id="4b961-141">Идентификатор коллекции в SCCM.</span><span class="sxs-lookup"><span data-stu-id="4b961-141">The collection identifier in SCCM.</span></span>|
|<span data-ttu-id="4b961-142">хиерарчинаме</span><span class="sxs-lookup"><span data-stu-id="4b961-142">hierarchyName</span></span>|<span data-ttu-id="4b961-143">String</span><span class="sxs-lookup"><span data-stu-id="4b961-143">String</span></span>|<span data-ttu-id="4b961-144">Хиерарчинаме.</span><span class="sxs-lookup"><span data-stu-id="4b961-144">The HierarchyName.</span></span>|
|<span data-ttu-id="4b961-145">хиерарчидентифиер</span><span class="sxs-lookup"><span data-stu-id="4b961-145">hierarchyIdentifier</span></span>|<span data-ttu-id="4b961-146">String</span><span class="sxs-lookup"><span data-stu-id="4b961-146">String</span></span>|<span data-ttu-id="4b961-147">Идентификатор иерархии.</span><span class="sxs-lookup"><span data-stu-id="4b961-147">The Hierarchy Identifier.</span></span>|
|<span data-ttu-id="4b961-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b961-148">createdDateTime</span></span>|<span data-ttu-id="4b961-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b961-149">DateTimeOffset</span></span>|<span data-ttu-id="4b961-150">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="4b961-150">The created date.</span></span>|
|<span data-ttu-id="4b961-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b961-151">lastModifiedDateTime</span></span>|<span data-ttu-id="4b961-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b961-152">DateTimeOffset</span></span>|<span data-ttu-id="4b961-153">Дата последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="4b961-153">The last modified date.</span></span>|



## <a name="response"></a><span data-ttu-id="4b961-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b961-154">Response</span></span>
<span data-ttu-id="4b961-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b961-155">If successful, this method returns a `200 OK` response code and an updated [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b961-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4b961-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b961-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b961-157">Request</span></span>
<span data-ttu-id="4b961-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b961-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configManagerCollections/{configManagerCollectionId}
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

### <a name="response"></a><span data-ttu-id="4b961-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b961-159">Response</span></span>
<span data-ttu-id="4b961-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b961-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




