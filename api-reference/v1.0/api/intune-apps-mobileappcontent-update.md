---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 222ce1bfbe7ae0eda6c93c09874db5f93899ffa2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759695"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="9f5ae-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9f5ae-103">Update mobileAppContent</span></span>

<span data-ttu-id="9f5ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f5ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f5ae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f5ae-106">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="9f5ae-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f5ae-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f5ae-107">Prerequisites</span></span>
<span data-ttu-id="9f5ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f5ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f5ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f5ae-110">Permission type</span></span>|<span data-ttu-id="9f5ae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f5ae-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f5ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f5ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f5ae-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5ae-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f5ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f5ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f5ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-115">Not supported.</span></span>|
|<span data-ttu-id="9f5ae-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f5ae-116">Application</span></span>|<span data-ttu-id="9f5ae-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5ae-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f5ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f5ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="9f5ae-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f5ae-119">Request headers</span></span>
|<span data-ttu-id="9f5ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f5ae-120">Header</span></span>|<span data-ttu-id="9f5ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f5ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f5ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f5ae-122">Authorization</span></span>|<span data-ttu-id="9f5ae-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f5ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f5ae-124">Accept</span></span>|<span data-ttu-id="9f5ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f5ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f5ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f5ae-126">Request body</span></span>
<span data-ttu-id="9f5ae-127">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="9f5ae-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="9f5ae-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="9f5ae-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f5ae-129">Property</span></span>|<span data-ttu-id="9f5ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f5ae-130">Type</span></span>|<span data-ttu-id="9f5ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f5ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f5ae-132">id</span><span class="sxs-lookup"><span data-stu-id="9f5ae-132">id</span></span>|<span data-ttu-id="9f5ae-133">String</span><span class="sxs-lookup"><span data-stu-id="9f5ae-133">String</span></span>|<span data-ttu-id="9f5ae-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="9f5ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5ae-135">Response</span></span>
<span data-ttu-id="9f5ae-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f5ae-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9f5ae-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f5ae-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f5ae-138">Request</span></span>
<span data-ttu-id="9f5ae-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="9f5ae-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5ae-140">Response</span></span>
<span data-ttu-id="9f5ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f5ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




