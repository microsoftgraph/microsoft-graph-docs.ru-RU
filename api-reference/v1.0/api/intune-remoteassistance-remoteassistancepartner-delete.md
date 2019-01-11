---
title: Удаление объекта remoteAssistancePartner
description: Удаляет объект remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d62f7bc9ba8da090fa62d93b78424c647d5e7f2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828667"
---
# <a name="delete-remoteassistancepartner"></a><span data-ttu-id="f1b07-103">Удаление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="f1b07-103">Delete remoteAssistancePartner</span></span>

> <span data-ttu-id="f1b07-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1b07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1b07-105">Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="f1b07-105">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1b07-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1b07-106">Prerequisites</span></span>
<span data-ttu-id="f1b07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1b07-109">Permission type</span></span>|<span data-ttu-id="f1b07-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1b07-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1b07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1b07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1b07-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b07-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1b07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1b07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1b07-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1b07-114">Not supported.</span></span>|
|<span data-ttu-id="f1b07-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1b07-115">Application</span></span>|<span data-ttu-id="f1b07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1b07-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1b07-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1b07-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="f1b07-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1b07-118">Request headers</span></span>
|<span data-ttu-id="f1b07-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1b07-119">Header</span></span>|<span data-ttu-id="f1b07-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f1b07-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1b07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b07-121">Authorization</span></span>|<span data-ttu-id="f1b07-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f1b07-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1b07-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1b07-123">Accept</span></span>|<span data-ttu-id="f1b07-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b07-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1b07-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1b07-125">Request body</span></span>
<span data-ttu-id="f1b07-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1b07-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1b07-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1b07-127">Response</span></span>
<span data-ttu-id="f1b07-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1b07-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1b07-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f1b07-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1b07-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1b07-130">Request</span></span>
<span data-ttu-id="f1b07-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1b07-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="f1b07-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1b07-132">Response</span></span>
<span data-ttu-id="f1b07-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f1b07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



