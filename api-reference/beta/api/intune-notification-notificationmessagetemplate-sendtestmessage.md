---
title: Действие sendTestMessage
description: Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 389fc976ab8394434f38173495b22d89112bca66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528983"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="82f82-103">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="82f82-103">sendTestMessage action</span></span>

> <span data-ttu-id="82f82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82f82-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f82-106">Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82f82-106">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82f82-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82f82-107">Prerequisites</span></span>
<span data-ttu-id="82f82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f82-110">Permission type</span></span>|<span data-ttu-id="82f82-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82f82-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f82-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82f82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f82-115">Not supported.</span></span>|
|<span data-ttu-id="82f82-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f82-116">Application</span></span>|<span data-ttu-id="82f82-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="82f82-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f82-119">Request headers</span></span>
|<span data-ttu-id="82f82-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82f82-120">Header</span></span>|<span data-ttu-id="82f82-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82f82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82f82-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82f82-122">Authorization</span></span>|<span data-ttu-id="82f82-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82f82-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82f82-124">Accept</span></span>|<span data-ttu-id="82f82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82f82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f82-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f82-126">Request body</span></span>
<span data-ttu-id="82f82-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82f82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f82-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="82f82-128">Response</span></span>
<span data-ttu-id="82f82-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82f82-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82f82-130">Пример</span><span class="sxs-lookup"><span data-stu-id="82f82-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="82f82-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f82-131">Request</span></span>
<span data-ttu-id="82f82-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f82-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="82f82-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f82-133">Response</span></span>
<span data-ttu-id="82f82-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





