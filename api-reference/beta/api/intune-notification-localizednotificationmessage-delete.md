---
title: Удаление localizedNotificationMessage
description: Удаляет объект localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98a95da5f93b899448668c4c7cb387ab18efefc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462749"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="ff249-103">Удаление localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="ff249-103">Delete localizedNotificationMessage</span></span>

<span data-ttu-id="ff249-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff249-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff249-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff249-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff249-107">Удаляет объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="ff249-107">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff249-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff249-108">Prerequisites</span></span>
<span data-ttu-id="ff249-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff249-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff249-111">Permission type</span></span>|<span data-ttu-id="ff249-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff249-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff249-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff249-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff249-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff249-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff249-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff249-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff249-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff249-116">Not supported.</span></span>|
|<span data-ttu-id="ff249-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff249-117">Application</span></span>|<span data-ttu-id="ff249-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff249-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff249-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff249-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="ff249-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff249-120">Request headers</span></span>
|<span data-ttu-id="ff249-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff249-121">Header</span></span>|<span data-ttu-id="ff249-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff249-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff249-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff249-123">Authorization</span></span>|<span data-ttu-id="ff249-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff249-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff249-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff249-125">Accept</span></span>|<span data-ttu-id="ff249-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff249-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff249-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff249-127">Request body</span></span>
<span data-ttu-id="ff249-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff249-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff249-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff249-129">Response</span></span>
<span data-ttu-id="ff249-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff249-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff249-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ff249-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff249-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff249-132">Request</span></span>
<span data-ttu-id="ff249-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff249-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="ff249-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff249-134">Response</span></span>
<span data-ttu-id="ff249-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff249-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





