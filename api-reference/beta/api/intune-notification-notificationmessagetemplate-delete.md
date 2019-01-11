---
title: Удаление notificationMessageTemplate
description: Удаление объекта notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6d40b936678cb6fd8eeaa05ab3136f27731e943c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816410"
---
# <a name="delete-notificationmessagetemplate"></a><span data-ttu-id="50c31-103">Удаление notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="50c31-103">Delete notificationMessageTemplate</span></span>

> <span data-ttu-id="50c31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50c31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50c31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50c31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50c31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50c31-107">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="50c31-107">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50c31-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50c31-108">Prerequisites</span></span>
<span data-ttu-id="50c31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50c31-111">Permission type</span></span>|<span data-ttu-id="50c31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50c31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50c31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50c31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50c31-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c31-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50c31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50c31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50c31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c31-116">Not supported.</span></span>|
|<span data-ttu-id="50c31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50c31-117">Application</span></span>|<span data-ttu-id="50c31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50c31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50c31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="50c31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50c31-120">Request headers</span></span>
|<span data-ttu-id="50c31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50c31-121">Header</span></span>|<span data-ttu-id="50c31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50c31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50c31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c31-123">Authorization</span></span>|<span data-ttu-id="50c31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="50c31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50c31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50c31-125">Accept</span></span>|<span data-ttu-id="50c31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50c31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50c31-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50c31-127">Request body</span></span>
<span data-ttu-id="50c31-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50c31-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50c31-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="50c31-129">Response</span></span>
<span data-ttu-id="50c31-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50c31-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50c31-131">Пример</span><span class="sxs-lookup"><span data-stu-id="50c31-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="50c31-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c31-132">Request</span></span>
<span data-ttu-id="50c31-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50c31-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="50c31-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="50c31-134">Response</span></span>
<span data-ttu-id="50c31-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="50c31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





