---
title: Действие sendTestMessage
description: Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.
author: tfitzmac
ms.openlocfilehash: 4495b4064f18739744d0f1f5f8709f28373d5f89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362757"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="f587e-103">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="f587e-103">sendTestMessage action</span></span>

> <span data-ttu-id="f587e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f587e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f587e-105">Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f587e-105">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f587e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f587e-106">Prerequisites</span></span>
<span data-ttu-id="f587e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f587e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f587e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f587e-109">Permission type</span></span>|<span data-ttu-id="f587e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f587e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f587e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f587e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f587e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f587e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f587e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f587e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f587e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f587e-114">Not supported.</span></span>|
|<span data-ttu-id="f587e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f587e-115">Application</span></span>|<span data-ttu-id="f587e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f587e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f587e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f587e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="f587e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f587e-118">Request headers</span></span>
|<span data-ttu-id="f587e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f587e-119">Header</span></span>|<span data-ttu-id="f587e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f587e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f587e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f587e-121">Authorization</span></span>|<span data-ttu-id="f587e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f587e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f587e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f587e-123">Accept</span></span>|<span data-ttu-id="f587e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f587e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f587e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f587e-125">Request body</span></span>
<span data-ttu-id="f587e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f587e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f587e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f587e-127">Response</span></span>
<span data-ttu-id="f587e-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f587e-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f587e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f587e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f587e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f587e-130">Request</span></span>
<span data-ttu-id="f587e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f587e-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="f587e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f587e-132">Response</span></span>
<span data-ttu-id="f587e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f587e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



