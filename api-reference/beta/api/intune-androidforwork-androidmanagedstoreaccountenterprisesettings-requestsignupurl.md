---
title: Действие requestSignupUrl
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ad71729dedce49b7bfd50d31dbacae64b59a8c17
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401819"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="f7dd5-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="f7dd5-103">requestSignupUrl action</span></span>

> <span data-ttu-id="f7dd5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7dd5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7dd5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7dd5-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7dd5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7dd5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7dd5-108">Prerequisites</span></span>
<span data-ttu-id="f7dd5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7dd5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7dd5-111">Permission type</span></span>|<span data-ttu-id="f7dd5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7dd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7dd5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7dd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7dd5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7dd5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7dd5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7dd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7dd5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-116">Not supported.</span></span>|
|<span data-ttu-id="f7dd5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7dd5-117">Application</span></span>|<span data-ttu-id="f7dd5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7dd5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7dd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="f7dd5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7dd5-120">Request headers</span></span>
|<span data-ttu-id="f7dd5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7dd5-121">Header</span></span>|<span data-ttu-id="f7dd5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7dd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7dd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7dd5-123">Authorization</span></span>|<span data-ttu-id="f7dd5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7dd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7dd5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7dd5-125">Accept</span></span>|<span data-ttu-id="f7dd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7dd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7dd5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7dd5-127">Request body</span></span>
<span data-ttu-id="f7dd5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7dd5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7dd5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7dd5-130">Property</span></span>|<span data-ttu-id="f7dd5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7dd5-131">Type</span></span>|<span data-ttu-id="f7dd5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7dd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7dd5-133">hostName</span><span class="sxs-lookup"><span data-stu-id="f7dd5-133">hostName</span></span>|<span data-ttu-id="f7dd5-134">String</span><span class="sxs-lookup"><span data-stu-id="f7dd5-134">String</span></span>|<span data-ttu-id="f7dd5-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7dd5-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7dd5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7dd5-136">Response</span></span>
<span data-ttu-id="f7dd5-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7dd5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f7dd5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7dd5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7dd5-139">Request</span></span>
<span data-ttu-id="f7dd5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="f7dd5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7dd5-141">Response</span></span>
<span data-ttu-id="f7dd5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7dd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




