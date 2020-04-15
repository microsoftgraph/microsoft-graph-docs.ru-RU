---
title: Get notificationMessageTemplate
description: Чтение свойств и связей объекта notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6eeb72577bba65b86290fe5d23604c275f3ebf35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452979"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="c764e-103">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c764e-103">Get notificationMessageTemplate</span></span>

<span data-ttu-id="c764e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c764e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c764e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c764e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c764e-106">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c764e-106">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c764e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c764e-107">Prerequisites</span></span>
<span data-ttu-id="c764e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c764e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c764e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c764e-110">Permission type</span></span>|<span data-ttu-id="c764e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c764e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c764e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c764e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c764e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c764e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c764e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c764e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c764e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c764e-115">Not supported.</span></span>|
|<span data-ttu-id="c764e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c764e-116">Application</span></span>|<span data-ttu-id="c764e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c764e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c764e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c764e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c764e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c764e-119">Optional query parameters</span></span>
<span data-ttu-id="c764e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c764e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c764e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c764e-121">Request headers</span></span>
|<span data-ttu-id="c764e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c764e-122">Header</span></span>|<span data-ttu-id="c764e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c764e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c764e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c764e-124">Authorization</span></span>|<span data-ttu-id="c764e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c764e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c764e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c764e-126">Accept</span></span>|<span data-ttu-id="c764e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c764e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c764e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c764e-128">Request body</span></span>
<span data-ttu-id="c764e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c764e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c764e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c764e-130">Response</span></span>
<span data-ttu-id="c764e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c764e-131">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c764e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c764e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c764e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c764e-133">Request</span></span>
<span data-ttu-id="c764e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c764e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="c764e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c764e-135">Response</span></span>
<span data-ttu-id="c764e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c764e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo"
  }
}
```






