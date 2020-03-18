---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f51179978586ff309b3c7f42fca766a096ea451
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761358"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="cfcfe-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cfcfe-103">Create mobileAppContent</span></span>

> <span data-ttu-id="cfcfe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfcfe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfcfe-106">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cfcfe-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfcfe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cfcfe-107">Prerequisites</span></span>
<span data-ttu-id="cfcfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfcfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfcfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcfe-110">Permission type</span></span>|<span data-ttu-id="cfcfe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfcfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfcfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfcfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfcfe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfcfe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cfcfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfcfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfcfe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-115">Not supported.</span></span>|
|<span data-ttu-id="cfcfe-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cfcfe-116">Application</span></span>|<span data-ttu-id="cfcfe-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfcfe-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfcfe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfcfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="cfcfe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cfcfe-119">Request headers</span></span>
|<span data-ttu-id="cfcfe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cfcfe-120">Header</span></span>|<span data-ttu-id="cfcfe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cfcfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfcfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfcfe-122">Authorization</span></span>|<span data-ttu-id="cfcfe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfcfe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cfcfe-124">Accept</span></span>|<span data-ttu-id="cfcfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfcfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfcfe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfcfe-126">Request body</span></span>
<span data-ttu-id="cfcfe-127">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="cfcfe-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="cfcfe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfcfe-129">Property</span></span>|<span data-ttu-id="cfcfe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cfcfe-130">Type</span></span>|<span data-ttu-id="cfcfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cfcfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfcfe-132">id</span><span class="sxs-lookup"><span data-stu-id="cfcfe-132">id</span></span>|<span data-ttu-id="cfcfe-133">String</span><span class="sxs-lookup"><span data-stu-id="cfcfe-133">String</span></span>|<span data-ttu-id="cfcfe-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="cfcfe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcfe-135">Response</span></span>
<span data-ttu-id="cfcfe-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfcfe-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cfcfe-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfcfe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfcfe-138">Request</span></span>
<span data-ttu-id="cfcfe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="cfcfe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcfe-140">Response</span></span>
<span data-ttu-id="cfcfe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




