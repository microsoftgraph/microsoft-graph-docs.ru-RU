---
title: Удаление notificationMessageTemplate
description: Удаление объекта notificationMessageTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33d4c2f0cbc0a9b60b2d6428911e69cf616af4e8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362830"
---
# <a name="delete-notificationmessagetemplate"></a><span data-ttu-id="957bb-103">Удаление notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="957bb-103">Delete notificationMessageTemplate</span></span>

> <span data-ttu-id="957bb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="957bb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="957bb-105">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="957bb-105">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="957bb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="957bb-106">Prerequisites</span></span>
<span data-ttu-id="957bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="957bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="957bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="957bb-109">Permission type</span></span>|<span data-ttu-id="957bb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="957bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="957bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="957bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="957bb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957bb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="957bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="957bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="957bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="957bb-114">Not supported.</span></span>|
|<span data-ttu-id="957bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="957bb-115">Application</span></span>|<span data-ttu-id="957bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="957bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="957bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="957bb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="957bb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="957bb-118">Request headers</span></span>
|<span data-ttu-id="957bb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="957bb-119">Header</span></span>|<span data-ttu-id="957bb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="957bb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="957bb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="957bb-121">Authorization</span></span>|<span data-ttu-id="957bb-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="957bb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="957bb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="957bb-123">Accept</span></span>|<span data-ttu-id="957bb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="957bb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="957bb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="957bb-125">Request body</span></span>
<span data-ttu-id="957bb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="957bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="957bb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="957bb-127">Response</span></span>
<span data-ttu-id="957bb-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="957bb-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="957bb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="957bb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="957bb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="957bb-130">Request</span></span>
<span data-ttu-id="957bb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="957bb-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="957bb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="957bb-132">Response</span></span>
<span data-ttu-id="957bb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="957bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




