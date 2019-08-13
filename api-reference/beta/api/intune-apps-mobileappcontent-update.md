---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1232e2d4ee739c1fc41257345e9d7cacd57c6764
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329238"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="10011-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="10011-103">Update mobileAppContent</span></span>

> <span data-ttu-id="10011-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10011-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10011-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10011-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10011-106">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="10011-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10011-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10011-107">Prerequisites</span></span>
<span data-ttu-id="10011-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10011-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10011-110">Permission type</span></span>|<span data-ttu-id="10011-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10011-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10011-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10011-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10011-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10011-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10011-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10011-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10011-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10011-115">Not supported.</span></span>|
|<span data-ttu-id="10011-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10011-116">Application</span></span>|<span data-ttu-id="10011-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10011-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10011-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10011-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="10011-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10011-119">Request headers</span></span>
|<span data-ttu-id="10011-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10011-120">Header</span></span>|<span data-ttu-id="10011-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10011-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10011-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10011-122">Authorization</span></span>|<span data-ttu-id="10011-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10011-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10011-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10011-124">Accept</span></span>|<span data-ttu-id="10011-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10011-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10011-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10011-126">Request body</span></span>
<span data-ttu-id="10011-127">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10011-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="10011-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="10011-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="10011-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10011-129">Property</span></span>|<span data-ttu-id="10011-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10011-130">Type</span></span>|<span data-ttu-id="10011-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10011-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10011-132">id</span><span class="sxs-lookup"><span data-stu-id="10011-132">id</span></span>|<span data-ttu-id="10011-133">String</span><span class="sxs-lookup"><span data-stu-id="10011-133">String</span></span>|<span data-ttu-id="10011-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="10011-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="10011-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="10011-135">Response</span></span>
<span data-ttu-id="10011-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10011-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10011-137">Пример</span><span class="sxs-lookup"><span data-stu-id="10011-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="10011-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="10011-138">Request</span></span>
<span data-ttu-id="10011-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10011-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="10011-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="10011-140">Response</span></span>
<span data-ttu-id="10011-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10011-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```






