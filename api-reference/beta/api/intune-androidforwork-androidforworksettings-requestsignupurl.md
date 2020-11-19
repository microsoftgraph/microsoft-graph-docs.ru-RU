---
title: Действие requestSignupUrl
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f696dde61e114171fc5af004d7d910066d52ee2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254737"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="2659b-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="2659b-103">requestSignupUrl action</span></span>

<span data-ttu-id="2659b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2659b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2659b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2659b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2659b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2659b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2659b-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2659b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2659b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2659b-108">Prerequisites</span></span>
<span data-ttu-id="2659b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2659b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2659b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2659b-111">Permission type</span></span>|<span data-ttu-id="2659b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2659b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2659b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2659b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2659b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2659b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2659b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2659b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2659b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2659b-116">Not supported.</span></span>|
|<span data-ttu-id="2659b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2659b-117">Application</span></span>|<span data-ttu-id="2659b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2659b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2659b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2659b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="2659b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2659b-120">Request headers</span></span>
|<span data-ttu-id="2659b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2659b-121">Header</span></span>|<span data-ttu-id="2659b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2659b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2659b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2659b-123">Authorization</span></span>|<span data-ttu-id="2659b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2659b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2659b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2659b-125">Accept</span></span>|<span data-ttu-id="2659b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2659b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2659b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2659b-127">Request body</span></span>
<span data-ttu-id="2659b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2659b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2659b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2659b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2659b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2659b-130">Property</span></span>|<span data-ttu-id="2659b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2659b-131">Type</span></span>|<span data-ttu-id="2659b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2659b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2659b-133">hostName</span><span class="sxs-lookup"><span data-stu-id="2659b-133">hostName</span></span>|<span data-ttu-id="2659b-134">String</span><span class="sxs-lookup"><span data-stu-id="2659b-134">String</span></span>|<span data-ttu-id="2659b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2659b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2659b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2659b-136">Response</span></span>
<span data-ttu-id="2659b-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2659b-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2659b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2659b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2659b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2659b-139">Request</span></span>
<span data-ttu-id="2659b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2659b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="2659b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2659b-141">Response</span></span>
<span data-ttu-id="2659b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2659b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




