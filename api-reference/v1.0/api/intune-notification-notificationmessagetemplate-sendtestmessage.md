---
title: Действие sendTestMessage
description: Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff59b9f50e7132f2e32d59a73257da0001289a38
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754848"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="1fc44-103">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="1fc44-103">sendTestMessage action</span></span>

<span data-ttu-id="1fc44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fc44-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fc44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fc44-106">Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1fc44-106">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fc44-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1fc44-107">Prerequisites</span></span>
<span data-ttu-id="1fc44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fc44-110">Permission type</span></span>|<span data-ttu-id="1fc44-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fc44-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fc44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fc44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fc44-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc44-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1fc44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fc44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fc44-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fc44-115">Not supported.</span></span>|
|<span data-ttu-id="1fc44-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1fc44-116">Application</span></span>|<span data-ttu-id="1fc44-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc44-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fc44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fc44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="1fc44-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fc44-119">Request headers</span></span>
|<span data-ttu-id="1fc44-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fc44-120">Header</span></span>|<span data-ttu-id="1fc44-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1fc44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fc44-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fc44-122">Authorization</span></span>|<span data-ttu-id="1fc44-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fc44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fc44-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1fc44-124">Accept</span></span>|<span data-ttu-id="1fc44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fc44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc44-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fc44-126">Request body</span></span>
<span data-ttu-id="1fc44-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fc44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fc44-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc44-128">Response</span></span>
<span data-ttu-id="1fc44-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1fc44-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1fc44-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1fc44-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fc44-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc44-131">Request</span></span>
<span data-ttu-id="1fc44-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fc44-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="1fc44-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc44-133">Response</span></span>
<span data-ttu-id="1fc44-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fc44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




