---
title: Действие requestSignupUrl
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d74dc1e018b0ff620715c080e64f0576ec2b3da1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153195"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="5cd12-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="5cd12-103">requestSignupUrl action</span></span>

> <span data-ttu-id="5cd12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cd12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd12-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5cd12-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd12-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5cd12-107">Prerequisites</span></span>
<span data-ttu-id="5cd12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cd12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cd12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cd12-110">Permission type</span></span>|<span data-ttu-id="5cd12-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cd12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd12-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cd12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd12-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd12-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5cd12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cd12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd12-115">Not supported.</span></span>|
|<span data-ttu-id="5cd12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cd12-116">Application</span></span>|<span data-ttu-id="5cd12-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cd12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="5cd12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cd12-119">Request headers</span></span>
|<span data-ttu-id="5cd12-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cd12-120">Header</span></span>|<span data-ttu-id="5cd12-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5cd12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cd12-122">Authorization</span></span>|<span data-ttu-id="5cd12-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5cd12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd12-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5cd12-124">Accept</span></span>|<span data-ttu-id="5cd12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd12-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cd12-126">Request body</span></span>
<span data-ttu-id="5cd12-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cd12-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5cd12-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5cd12-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5cd12-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cd12-129">Property</span></span>|<span data-ttu-id="5cd12-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5cd12-130">Type</span></span>|<span data-ttu-id="5cd12-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5cd12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cd12-132">hostName</span><span class="sxs-lookup"><span data-stu-id="5cd12-132">hostName</span></span>|<span data-ttu-id="5cd12-133">String</span><span class="sxs-lookup"><span data-stu-id="5cd12-133">String</span></span>|<span data-ttu-id="5cd12-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5cd12-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5cd12-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cd12-135">Response</span></span>
<span data-ttu-id="5cd12-136">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cd12-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd12-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5cd12-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd12-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cd12-138">Request</span></span>
<span data-ttu-id="5cd12-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cd12-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="5cd12-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cd12-140">Response</span></span>
<span data-ttu-id="5cd12-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5cd12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




