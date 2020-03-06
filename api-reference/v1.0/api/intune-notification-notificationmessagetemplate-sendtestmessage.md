---
title: Действие sendTestMessage
description: Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b14063b93ef8cd4b0b9e0fe5a42ee7e15f16d8fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512736"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="715fb-103">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="715fb-103">sendTestMessage action</span></span>

<span data-ttu-id="715fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="715fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="715fb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="715fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="715fb-106">Отправляет проверочное сообщение, используя указанный объект notificationMessageTemplate в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="715fb-106">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="715fb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="715fb-107">Prerequisites</span></span>
<span data-ttu-id="715fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="715fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="715fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="715fb-110">Permission type</span></span>|<span data-ttu-id="715fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="715fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="715fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="715fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="715fb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="715fb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="715fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="715fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="715fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="715fb-115">Not supported.</span></span>|
|<span data-ttu-id="715fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="715fb-116">Application</span></span>|<span data-ttu-id="715fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="715fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="715fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="715fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="715fb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="715fb-119">Request headers</span></span>
|<span data-ttu-id="715fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="715fb-120">Header</span></span>|<span data-ttu-id="715fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="715fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="715fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="715fb-122">Authorization</span></span>|<span data-ttu-id="715fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="715fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="715fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="715fb-124">Accept</span></span>|<span data-ttu-id="715fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="715fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="715fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="715fb-126">Request body</span></span>
<span data-ttu-id="715fb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="715fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="715fb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="715fb-128">Response</span></span>
<span data-ttu-id="715fb-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="715fb-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="715fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="715fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="715fb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="715fb-131">Request</span></span>
<span data-ttu-id="715fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="715fb-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="715fb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="715fb-133">Response</span></span>
<span data-ttu-id="715fb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="715fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




