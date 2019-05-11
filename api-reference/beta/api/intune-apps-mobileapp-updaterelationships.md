---
title: действие Упдатерелатионшипс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53035c756e346a8df68e81cd37877e6d4255348e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935344"
---
# <a name="updaterelationships-action"></a><span data-ttu-id="5b207-103">действие Упдатерелатионшипс</span><span class="sxs-lookup"><span data-stu-id="5b207-103">updateRelationships action</span></span>

> <span data-ttu-id="5b207-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b207-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b207-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b207-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b207-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b207-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b207-107">Prerequisites</span></span>
<span data-ttu-id="5b207-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b207-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b207-110">Permission type</span></span>|<span data-ttu-id="5b207-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b207-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b207-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b207-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b207-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b207-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b207-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b207-115">Not supported.</span></span>|
|<span data-ttu-id="5b207-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b207-116">Application</span></span>|<span data-ttu-id="5b207-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b207-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b207-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/updateRelationships
```

## <a name="request-headers"></a><span data-ttu-id="5b207-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b207-119">Request headers</span></span>
|<span data-ttu-id="5b207-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b207-120">Header</span></span>|<span data-ttu-id="5b207-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b207-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b207-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b207-122">Authorization</span></span>|<span data-ttu-id="5b207-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b207-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b207-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b207-124">Accept</span></span>|<span data-ttu-id="5b207-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b207-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b207-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b207-126">Request body</span></span>
<span data-ttu-id="5b207-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b207-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5b207-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5b207-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5b207-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b207-129">Property</span></span>|<span data-ttu-id="5b207-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b207-130">Type</span></span>|<span data-ttu-id="5b207-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b207-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b207-132">Таблица</span><span class="sxs-lookup"><span data-stu-id="5b207-132">relationships</span></span>|<span data-ttu-id="5b207-133">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5b207-133">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="5b207-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5b207-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5b207-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b207-135">Response</span></span>
<span data-ttu-id="5b207-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b207-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b207-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5b207-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b207-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b207-138">Request</span></span>
<span data-ttu-id="5b207-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b207-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships

Content-type: application/json
Content-length: 256

{
  "relationships": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5b207-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b207-140">Response</span></span>
<span data-ttu-id="5b207-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b207-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




