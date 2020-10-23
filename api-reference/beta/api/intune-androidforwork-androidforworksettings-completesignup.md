---
title: Действие completeSignup
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45210c990925c7946e80714e0ed98a6d58cce83a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701132"
---
# <a name="completesignup-action"></a><span data-ttu-id="f61d8-103">Действие completeSignup</span><span class="sxs-lookup"><span data-stu-id="f61d8-103">completeSignup action</span></span>

<span data-ttu-id="f61d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f61d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f61d8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f61d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f61d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f61d8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f61d8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f61d8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f61d8-108">Prerequisites</span></span>
<span data-ttu-id="f61d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f61d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f61d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f61d8-111">Permission type</span></span>|<span data-ttu-id="f61d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f61d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f61d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f61d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f61d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f61d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f61d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f61d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f61d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61d8-116">Not supported.</span></span>|
|<span data-ttu-id="f61d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f61d8-117">Application</span></span>|<span data-ttu-id="f61d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f61d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f61d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f61d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="f61d8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f61d8-120">Request headers</span></span>
|<span data-ttu-id="f61d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f61d8-121">Header</span></span>|<span data-ttu-id="f61d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f61d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f61d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f61d8-123">Authorization</span></span>|<span data-ttu-id="f61d8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f61d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f61d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f61d8-125">Accept</span></span>|<span data-ttu-id="f61d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f61d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f61d8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f61d8-127">Request body</span></span>
<span data-ttu-id="f61d8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f61d8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f61d8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f61d8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f61d8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f61d8-130">Property</span></span>|<span data-ttu-id="f61d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f61d8-131">Type</span></span>|<span data-ttu-id="f61d8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f61d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f61d8-133">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="f61d8-133">enterpriseToken</span></span>|<span data-ttu-id="f61d8-134">String</span><span class="sxs-lookup"><span data-stu-id="f61d8-134">String</span></span>|<span data-ttu-id="f61d8-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f61d8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f61d8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f61d8-136">Response</span></span>
<span data-ttu-id="f61d8-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f61d8-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f61d8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f61d8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f61d8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f61d8-139">Request</span></span>
<span data-ttu-id="f61d8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f61d8-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="f61d8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f61d8-141">Response</span></span>
<span data-ttu-id="f61d8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f61d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





