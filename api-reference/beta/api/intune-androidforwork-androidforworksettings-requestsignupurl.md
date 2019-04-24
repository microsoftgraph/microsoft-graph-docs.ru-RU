---
title: Действие requestSignupUrl
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f95b287b22681735d6529ee4833c846c673a2de1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498944"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="be51d-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="be51d-103">requestSignupUrl action</span></span>

> <span data-ttu-id="be51d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be51d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be51d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be51d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be51d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be51d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be51d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="be51d-107">Prerequisites</span></span>
<span data-ttu-id="be51d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be51d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be51d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be51d-110">Permission type</span></span>|<span data-ttu-id="be51d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be51d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be51d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be51d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be51d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be51d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be51d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be51d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be51d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be51d-115">Not supported.</span></span>|
|<span data-ttu-id="be51d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be51d-116">Application</span></span>|<span data-ttu-id="be51d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be51d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be51d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be51d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="be51d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be51d-119">Request headers</span></span>
|<span data-ttu-id="be51d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be51d-120">Header</span></span>|<span data-ttu-id="be51d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be51d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be51d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be51d-122">Authorization</span></span>|<span data-ttu-id="be51d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be51d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be51d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be51d-124">Accept</span></span>|<span data-ttu-id="be51d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be51d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be51d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be51d-126">Request body</span></span>
<span data-ttu-id="be51d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be51d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="be51d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="be51d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="be51d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be51d-129">Property</span></span>|<span data-ttu-id="be51d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be51d-130">Type</span></span>|<span data-ttu-id="be51d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be51d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be51d-132">hostName</span><span class="sxs-lookup"><span data-stu-id="be51d-132">hostName</span></span>|<span data-ttu-id="be51d-133">String</span><span class="sxs-lookup"><span data-stu-id="be51d-133">String</span></span>|<span data-ttu-id="be51d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be51d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="be51d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="be51d-135">Response</span></span>
<span data-ttu-id="be51d-136">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be51d-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be51d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="be51d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="be51d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="be51d-138">Request</span></span>
<span data-ttu-id="be51d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be51d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="be51d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="be51d-140">Response</span></span>
<span data-ttu-id="be51d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be51d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





