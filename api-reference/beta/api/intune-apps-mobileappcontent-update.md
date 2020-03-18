---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: edf11e64c7e5f21f6de528353a2e33175b61e968
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761330"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="679ca-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="679ca-103">Update mobileAppContent</span></span>

> <span data-ttu-id="679ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="679ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="679ca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="679ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="679ca-106">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="679ca-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="679ca-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="679ca-107">Prerequisites</span></span>
<span data-ttu-id="679ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="679ca-110">Permission type</span></span>|<span data-ttu-id="679ca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="679ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="679ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="679ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="679ca-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679ca-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="679ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="679ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="679ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="679ca-115">Not supported.</span></span>|
|<span data-ttu-id="679ca-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="679ca-116">Application</span></span>|<span data-ttu-id="679ca-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679ca-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="679ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="679ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="679ca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="679ca-119">Request headers</span></span>
|<span data-ttu-id="679ca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="679ca-120">Header</span></span>|<span data-ttu-id="679ca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="679ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="679ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="679ca-122">Authorization</span></span>|<span data-ttu-id="679ca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="679ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="679ca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="679ca-124">Accept</span></span>|<span data-ttu-id="679ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="679ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="679ca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="679ca-126">Request body</span></span>
<span data-ttu-id="679ca-127">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="679ca-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="679ca-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="679ca-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="679ca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="679ca-129">Property</span></span>|<span data-ttu-id="679ca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="679ca-130">Type</span></span>|<span data-ttu-id="679ca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="679ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="679ca-132">id</span><span class="sxs-lookup"><span data-stu-id="679ca-132">id</span></span>|<span data-ttu-id="679ca-133">String</span><span class="sxs-lookup"><span data-stu-id="679ca-133">String</span></span>|<span data-ttu-id="679ca-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="679ca-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="679ca-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="679ca-135">Response</span></span>
<span data-ttu-id="679ca-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="679ca-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679ca-137">Пример</span><span class="sxs-lookup"><span data-stu-id="679ca-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="679ca-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="679ca-138">Request</span></span>
<span data-ttu-id="679ca-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="679ca-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="679ca-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="679ca-140">Response</span></span>
<span data-ttu-id="679ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="679ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




