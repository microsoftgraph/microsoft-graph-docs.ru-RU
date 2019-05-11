---
title: Действие setPriority
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81da933b3fb921f30e32dc5cbc71b24654d25772
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900518"
---
# <a name="setpriority-action"></a><span data-ttu-id="b7058-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="b7058-103">setPriority action</span></span>

> <span data-ttu-id="b7058-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7058-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7058-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7058-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7058-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b7058-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7058-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7058-107">Prerequisites</span></span>
<span data-ttu-id="b7058-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7058-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7058-110">Permission type</span></span>|<span data-ttu-id="b7058-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7058-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7058-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7058-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7058-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7058-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7058-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7058-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7058-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7058-115">Not supported.</span></span>|
|<span data-ttu-id="b7058-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7058-116">Application</span></span>|<span data-ttu-id="b7058-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7058-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7058-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7058-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="b7058-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7058-119">Request headers</span></span>
|<span data-ttu-id="b7058-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7058-120">Header</span></span>|<span data-ttu-id="b7058-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7058-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7058-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7058-122">Authorization</span></span>|<span data-ttu-id="b7058-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7058-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7058-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7058-124">Accept</span></span>|<span data-ttu-id="b7058-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7058-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7058-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7058-126">Request body</span></span>
<span data-ttu-id="b7058-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7058-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b7058-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b7058-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b7058-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7058-129">Property</span></span>|<span data-ttu-id="b7058-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7058-130">Type</span></span>|<span data-ttu-id="b7058-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7058-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7058-132">priority</span><span class="sxs-lookup"><span data-stu-id="b7058-132">priority</span></span>|<span data-ttu-id="b7058-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b7058-133">Int32</span></span>|<span data-ttu-id="b7058-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b7058-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b7058-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7058-135">Response</span></span>
<span data-ttu-id="b7058-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b7058-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7058-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b7058-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7058-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7058-138">Request</span></span>
<span data-ttu-id="b7058-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7058-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="b7058-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7058-140">Response</span></span>
<span data-ttu-id="b7058-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




