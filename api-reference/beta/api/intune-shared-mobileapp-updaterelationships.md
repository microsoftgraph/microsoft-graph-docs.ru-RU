---
title: действие Упдатерелатионшипс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9626895c7df4a8e8ccac0bc999752c797b9e0b7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201007"
---
# <a name="updaterelationships-action"></a><span data-ttu-id="79959-103">действие Упдатерелатионшипс</span><span class="sxs-lookup"><span data-stu-id="79959-103">updateRelationships action</span></span>

> <span data-ttu-id="79959-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79959-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79959-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79959-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79959-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="79959-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79959-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79959-107">Prerequisites</span></span>
<span data-ttu-id="79959-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79959-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79959-110">Permission type</span></span>|<span data-ttu-id="79959-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79959-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79959-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79959-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="79959-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="79959-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="79959-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79959-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79959-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79959-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79959-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79959-116">Not supported.</span></span>|
|<span data-ttu-id="79959-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79959-117">Application</span></span>||
| <span data-ttu-id="79959-118">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="79959-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="79959-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79959-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79959-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79959-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/updateRelationships
```

## <a name="request-headers"></a><span data-ttu-id="79959-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79959-121">Request headers</span></span>
|<span data-ttu-id="79959-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79959-122">Header</span></span>|<span data-ttu-id="79959-123">Значение</span><span class="sxs-lookup"><span data-stu-id="79959-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79959-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79959-124">Authorization</span></span>|<span data-ttu-id="79959-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79959-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79959-126">Accept</span><span class="sxs-lookup"><span data-stu-id="79959-126">Accept</span></span>|<span data-ttu-id="79959-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79959-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79959-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79959-128">Request body</span></span>
<span data-ttu-id="79959-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79959-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="79959-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="79959-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="79959-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="79959-131">Property</span></span>|<span data-ttu-id="79959-132">Тип</span><span class="sxs-lookup"><span data-stu-id="79959-132">Type</span></span>|<span data-ttu-id="79959-133">Описание</span><span class="sxs-lookup"><span data-stu-id="79959-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79959-134">Таблица</span><span class="sxs-lookup"><span data-stu-id="79959-134">relationships</span></span>|<span data-ttu-id="79959-135">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="79959-135">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="79959-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="79959-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="79959-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="79959-137">Response</span></span>
<span data-ttu-id="79959-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79959-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79959-139">Пример</span><span class="sxs-lookup"><span data-stu-id="79959-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="79959-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="79959-140">Request</span></span>
<span data-ttu-id="79959-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79959-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79959-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="79959-142">Response</span></span>
<span data-ttu-id="79959-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79959-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




