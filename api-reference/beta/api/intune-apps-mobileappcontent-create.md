---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33211ab51c6009092dd3d00f830cac6693824e47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977469"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="2268f-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2268f-103">Create mobileAppContent</span></span>

<span data-ttu-id="2268f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2268f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2268f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2268f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2268f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2268f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2268f-107">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2268f-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2268f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2268f-108">Prerequisites</span></span>
<span data-ttu-id="2268f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2268f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2268f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2268f-111">Permission type</span></span>|<span data-ttu-id="2268f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2268f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2268f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2268f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2268f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2268f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2268f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2268f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2268f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2268f-116">Not supported.</span></span>|
|<span data-ttu-id="2268f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2268f-117">Application</span></span>|<span data-ttu-id="2268f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2268f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2268f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2268f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="2268f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2268f-120">Request headers</span></span>
|<span data-ttu-id="2268f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2268f-121">Header</span></span>|<span data-ttu-id="2268f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2268f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2268f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2268f-123">Authorization</span></span>|<span data-ttu-id="2268f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2268f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2268f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2268f-125">Accept</span></span>|<span data-ttu-id="2268f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2268f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2268f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2268f-127">Request body</span></span>
<span data-ttu-id="2268f-128">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2268f-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="2268f-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="2268f-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="2268f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2268f-130">Property</span></span>|<span data-ttu-id="2268f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2268f-131">Type</span></span>|<span data-ttu-id="2268f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2268f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2268f-133">id</span><span class="sxs-lookup"><span data-stu-id="2268f-133">id</span></span>|<span data-ttu-id="2268f-134">String</span><span class="sxs-lookup"><span data-stu-id="2268f-134">String</span></span>|<span data-ttu-id="2268f-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="2268f-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="2268f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2268f-136">Response</span></span>
<span data-ttu-id="2268f-137">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2268f-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2268f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2268f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2268f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2268f-139">Request</span></span>
<span data-ttu-id="2268f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2268f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="2268f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2268f-141">Response</span></span>
<span data-ttu-id="2268f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2268f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```






