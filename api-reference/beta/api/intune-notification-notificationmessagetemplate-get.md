---
title: Get notificationMessageTemplate
description: Чтение свойств и связей объекта notificationMessageTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c0263ab83f91ef5eca984f547d9c82577eb1656
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803142"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="2a2cc-103">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="2a2cc-103">Get notificationMessageTemplate</span></span>

> <span data-ttu-id="2a2cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a2cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a2cc-106">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2a2cc-106">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a2cc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2a2cc-107">Prerequisites</span></span>
<span data-ttu-id="2a2cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a2cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a2cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a2cc-110">Permission type</span></span>|<span data-ttu-id="2a2cc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a2cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a2cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a2cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a2cc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a2cc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2a2cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a2cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a2cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-115">Not supported.</span></span>|
|<span data-ttu-id="2a2cc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a2cc-116">Application</span></span>|<span data-ttu-id="2a2cc-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a2cc-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a2cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a2cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a2cc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a2cc-119">Optional query parameters</span></span>
<span data-ttu-id="2a2cc-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a2cc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a2cc-121">Request headers</span></span>
|<span data-ttu-id="2a2cc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a2cc-122">Header</span></span>|<span data-ttu-id="2a2cc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2a2cc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a2cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a2cc-124">Authorization</span></span>|<span data-ttu-id="2a2cc-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a2cc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2a2cc-126">Accept</span></span>|<span data-ttu-id="2a2cc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a2cc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a2cc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a2cc-128">Request body</span></span>
<span data-ttu-id="2a2cc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a2cc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a2cc-130">Response</span></span>
<span data-ttu-id="2a2cc-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-131">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a2cc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2a2cc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a2cc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a2cc-133">Request</span></span>
<span data-ttu-id="2a2cc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="2a2cc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a2cc-135">Response</span></span>
<span data-ttu-id="2a2cc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a2cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




