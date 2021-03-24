---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff40470d0313cc3b3d1f040b605069b1491d5a99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139827"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="ff155-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff155-103">Update mobileAppContent</span></span>

<span data-ttu-id="ff155-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff155-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff155-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff155-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff155-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff155-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff155-107">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ff155-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff155-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff155-108">Prerequisites</span></span>
<span data-ttu-id="ff155-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff155-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff155-111">Permission type</span></span>|<span data-ttu-id="ff155-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff155-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff155-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff155-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff155-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff155-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff155-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff155-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff155-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff155-116">Not supported.</span></span>|
|<span data-ttu-id="ff155-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff155-117">Application</span></span>|<span data-ttu-id="ff155-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff155-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff155-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff155-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="ff155-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff155-120">Request headers</span></span>
|<span data-ttu-id="ff155-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff155-121">Header</span></span>|<span data-ttu-id="ff155-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff155-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff155-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff155-123">Authorization</span></span>|<span data-ttu-id="ff155-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff155-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff155-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff155-125">Accept</span></span>|<span data-ttu-id="ff155-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff155-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff155-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff155-127">Request body</span></span>
<span data-ttu-id="ff155-128">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff155-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="ff155-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ff155-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="ff155-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff155-130">Property</span></span>|<span data-ttu-id="ff155-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff155-131">Type</span></span>|<span data-ttu-id="ff155-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff155-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff155-133">id</span><span class="sxs-lookup"><span data-stu-id="ff155-133">id</span></span>|<span data-ttu-id="ff155-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ff155-134">String</span></span>|<span data-ttu-id="ff155-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ff155-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="ff155-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff155-136">Response</span></span>
<span data-ttu-id="ff155-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff155-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff155-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ff155-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff155-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff155-139">Request</span></span>
<span data-ttu-id="ff155-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff155-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="ff155-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff155-141">Response</span></span>
<span data-ttu-id="ff155-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff155-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




