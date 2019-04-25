---
title: Удаление localizedNotificationMessage
description: Удаляет объект localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 800da6a7b73e9e952b83775f5c5b698dea6d0d2b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529284"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="98146-103">Удаление localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="98146-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="98146-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98146-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98146-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98146-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98146-106">Удаляет объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="98146-106">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98146-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98146-107">Prerequisites</span></span>
<span data-ttu-id="98146-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98146-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98146-110">Permission type</span></span>|<span data-ttu-id="98146-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98146-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98146-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98146-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98146-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98146-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="98146-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98146-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98146-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98146-115">Not supported.</span></span>|
|<span data-ttu-id="98146-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98146-116">Application</span></span>|<span data-ttu-id="98146-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98146-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98146-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98146-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="98146-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98146-119">Request headers</span></span>
|<span data-ttu-id="98146-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98146-120">Header</span></span>|<span data-ttu-id="98146-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98146-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98146-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98146-122">Authorization</span></span>|<span data-ttu-id="98146-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98146-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98146-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98146-124">Accept</span></span>|<span data-ttu-id="98146-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98146-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98146-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98146-126">Request body</span></span>
<span data-ttu-id="98146-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98146-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98146-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="98146-128">Response</span></span>
<span data-ttu-id="98146-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98146-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98146-130">Пример</span><span class="sxs-lookup"><span data-stu-id="98146-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="98146-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="98146-131">Request</span></span>
<span data-ttu-id="98146-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98146-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="98146-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="98146-133">Response</span></span>
<span data-ttu-id="98146-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98146-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





