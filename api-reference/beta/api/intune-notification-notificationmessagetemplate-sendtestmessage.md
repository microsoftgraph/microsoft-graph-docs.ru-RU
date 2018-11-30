---
title: Действие sendTestMessage
description: Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.
ms.openlocfilehash: e64a3f6e392bf05c55287a4388019bbb8c8f2bbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078073"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="f8dd3-103">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="f8dd3-103">sendTestMessage action</span></span>

> <span data-ttu-id="f8dd3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8dd3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8dd3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8dd3-107">Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-107">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8dd3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8dd3-108">Prerequisites</span></span>
<span data-ttu-id="f8dd3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8dd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8dd3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8dd3-111">Permission type</span></span>|<span data-ttu-id="f8dd3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8dd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8dd3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8dd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8dd3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8dd3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f8dd3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8dd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8dd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-116">Not supported.</span></span>|
|<span data-ttu-id="f8dd3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8dd3-117">Application</span></span>|<span data-ttu-id="f8dd3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8dd3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8dd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="f8dd3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8dd3-120">Request headers</span></span>
|<span data-ttu-id="f8dd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8dd3-121">Header</span></span>|<span data-ttu-id="f8dd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8dd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8dd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8dd3-123">Authorization</span></span>|<span data-ttu-id="f8dd3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f8dd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8dd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8dd3-125">Accept</span></span>|<span data-ttu-id="f8dd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8dd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8dd3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8dd3-127">Request body</span></span>
<span data-ttu-id="f8dd3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8dd3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8dd3-129">Response</span></span>
<span data-ttu-id="f8dd3-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8dd3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8dd3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8dd3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8dd3-132">Request</span></span>
<span data-ttu-id="f8dd3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8dd3-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="f8dd3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8dd3-134">Response</span></span>
<span data-ttu-id="f8dd3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f8dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





