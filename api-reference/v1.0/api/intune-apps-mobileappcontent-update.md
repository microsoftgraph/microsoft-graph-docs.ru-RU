---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c2a3a1003ef2cd948778c84dc8dd8f204994ee1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987596"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="70dc0-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="70dc0-103">Update mobileAppContent</span></span>

> <span data-ttu-id="70dc0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70dc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70dc0-105">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="70dc0-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70dc0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="70dc0-106">Prerequisites</span></span>
<span data-ttu-id="70dc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70dc0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70dc0-109">Permission type</span></span>|<span data-ttu-id="70dc0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70dc0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70dc0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70dc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70dc0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70dc0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70dc0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70dc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70dc0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70dc0-114">Not supported.</span></span>|
|<span data-ttu-id="70dc0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70dc0-115">Application</span></span>|<span data-ttu-id="70dc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70dc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70dc0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70dc0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="70dc0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70dc0-118">Request headers</span></span>
|<span data-ttu-id="70dc0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70dc0-119">Header</span></span>|<span data-ttu-id="70dc0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="70dc0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70dc0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70dc0-121">Authorization</span></span>|<span data-ttu-id="70dc0-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70dc0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70dc0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="70dc0-123">Accept</span></span>|<span data-ttu-id="70dc0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70dc0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70dc0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70dc0-125">Request body</span></span>
<span data-ttu-id="70dc0-126">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70dc0-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="70dc0-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="70dc0-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="70dc0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="70dc0-128">Property</span></span>|<span data-ttu-id="70dc0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="70dc0-129">Type</span></span>|<span data-ttu-id="70dc0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="70dc0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70dc0-131">id</span><span class="sxs-lookup"><span data-stu-id="70dc0-131">id</span></span>|<span data-ttu-id="70dc0-132">String</span><span class="sxs-lookup"><span data-stu-id="70dc0-132">String</span></span>|<span data-ttu-id="70dc0-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="70dc0-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="70dc0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70dc0-134">Response</span></span>
<span data-ttu-id="70dc0-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70dc0-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70dc0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="70dc0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="70dc0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="70dc0-137">Request</span></span>
<span data-ttu-id="70dc0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70dc0-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="70dc0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="70dc0-139">Response</span></span>
<span data-ttu-id="70dc0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70dc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



