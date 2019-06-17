---
title: Удаление notificationMessageTemplate
description: Удаление объекта notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bbb5ccf9327cbf7a85bbee09d62bc3405814080
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963550"
---
# <a name="delete-notificationmessagetemplate"></a><span data-ttu-id="fe030-103">Удаление notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="fe030-103">Delete notificationMessageTemplate</span></span>

> <span data-ttu-id="fe030-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe030-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe030-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe030-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe030-106">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="fe030-106">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe030-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe030-107">Prerequisites</span></span>
<span data-ttu-id="fe030-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe030-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe030-110">Permission type</span></span>|<span data-ttu-id="fe030-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe030-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe030-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe030-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe030-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe030-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fe030-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe030-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe030-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe030-115">Not supported.</span></span>|
|<span data-ttu-id="fe030-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe030-116">Application</span></span>|<span data-ttu-id="fe030-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe030-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe030-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe030-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="fe030-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe030-119">Request headers</span></span>
|<span data-ttu-id="fe030-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe030-120">Header</span></span>|<span data-ttu-id="fe030-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe030-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe030-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe030-122">Authorization</span></span>|<span data-ttu-id="fe030-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe030-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe030-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe030-124">Accept</span></span>|<span data-ttu-id="fe030-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe030-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe030-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe030-126">Request body</span></span>
<span data-ttu-id="fe030-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe030-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe030-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe030-128">Response</span></span>
<span data-ttu-id="fe030-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fe030-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe030-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fe030-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe030-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe030-131">Request</span></span>
<span data-ttu-id="fe030-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe030-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="fe030-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe030-133">Response</span></span>
<span data-ttu-id="fe030-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe030-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





