---
title: Перечисление объектов notificationMessageTemplate
description: Список свойств и связей объектов notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d878278149393e4e183df733ec3b1645dc77722f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754855"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="6ff60-103">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="6ff60-103">List notificationMessageTemplates</span></span>

<span data-ttu-id="6ff60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ff60-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ff60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff60-106">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="6ff60-106">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ff60-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ff60-107">Prerequisites</span></span>
<span data-ttu-id="6ff60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff60-110">Permission type</span></span>|<span data-ttu-id="6ff60-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ff60-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ff60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ff60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ff60-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff60-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ff60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ff60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ff60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ff60-115">Not supported.</span></span>|
|<span data-ttu-id="6ff60-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ff60-116">Application</span></span>|<span data-ttu-id="6ff60-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff60-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ff60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ff60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="6ff60-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ff60-119">Request headers</span></span>
|<span data-ttu-id="6ff60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ff60-120">Header</span></span>|<span data-ttu-id="6ff60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ff60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ff60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ff60-122">Authorization</span></span>|<span data-ttu-id="6ff60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ff60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ff60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ff60-124">Accept</span></span>|<span data-ttu-id="6ff60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ff60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ff60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ff60-126">Request body</span></span>
<span data-ttu-id="6ff60-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ff60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ff60-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff60-128">Response</span></span>
<span data-ttu-id="6ff60-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ff60-129">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ff60-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6ff60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ff60-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ff60-131">Request</span></span>
<span data-ttu-id="6ff60-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ff60-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="6ff60-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff60-133">Response</span></span>
<span data-ttu-id="6ff60-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ff60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo"
    }
  ]
}
```




