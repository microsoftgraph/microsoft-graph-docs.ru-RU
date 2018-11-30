---
title: Действие setPriority
description: Н/Д
ms.openlocfilehash: 5c446dcc1951e459e736048d34218faee5745428
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027295"
---
# <a name="setpriority-action"></a><span data-ttu-id="aa190-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="aa190-103">setPriority action</span></span>

> <span data-ttu-id="aa190-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa190-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa190-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa190-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa190-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa190-106">Prerequisites</span></span>
<span data-ttu-id="aa190-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa190-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa190-109">Permission type</span></span>|<span data-ttu-id="aa190-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa190-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa190-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa190-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa190-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa190-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa190-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa190-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa190-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa190-114">Not supported.</span></span>|
|<span data-ttu-id="aa190-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa190-115">Application</span></span>|<span data-ttu-id="aa190-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa190-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa190-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa190-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="aa190-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa190-118">Request headers</span></span>
|<span data-ttu-id="aa190-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa190-119">Header</span></span>|<span data-ttu-id="aa190-120">Значение</span><span class="sxs-lookup"><span data-stu-id="aa190-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa190-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa190-121">Authorization</span></span>|<span data-ttu-id="aa190-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aa190-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa190-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aa190-123">Accept</span></span>|<span data-ttu-id="aa190-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aa190-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa190-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa190-125">Request body</span></span>
<span data-ttu-id="aa190-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa190-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aa190-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aa190-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa190-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa190-128">Property</span></span>|<span data-ttu-id="aa190-129">Тип</span><span class="sxs-lookup"><span data-stu-id="aa190-129">Type</span></span>|<span data-ttu-id="aa190-130">Описание</span><span class="sxs-lookup"><span data-stu-id="aa190-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa190-131">priority</span><span class="sxs-lookup"><span data-stu-id="aa190-131">priority</span></span>|<span data-ttu-id="aa190-132">Int32</span><span class="sxs-lookup"><span data-stu-id="aa190-132">Int32</span></span>|<span data-ttu-id="aa190-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa190-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aa190-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa190-134">Response</span></span>
<span data-ttu-id="aa190-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aa190-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa190-136">Пример</span><span class="sxs-lookup"><span data-stu-id="aa190-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa190-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa190-137">Request</span></span>
<span data-ttu-id="aa190-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa190-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="aa190-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa190-139">Response</span></span>
<span data-ttu-id="aa190-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="aa190-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



