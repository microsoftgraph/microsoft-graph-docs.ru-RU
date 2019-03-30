---
title: Действие setPriority
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d73c6db0ec94bff8eca72dbcf900b9e3b1e56da1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989143"
---
# <a name="setpriority-action"></a><span data-ttu-id="6e5a5-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="6e5a5-103">setPriority action</span></span>

> <span data-ttu-id="6e5a5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e5a5-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e5a5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6e5a5-106">Prerequisites</span></span>
<span data-ttu-id="6e5a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e5a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e5a5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e5a5-109">Permission type</span></span>|<span data-ttu-id="6e5a5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e5a5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e5a5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e5a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e5a5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e5a5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e5a5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e5a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e5a5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-114">Not supported.</span></span>|
|<span data-ttu-id="6e5a5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e5a5-115">Application</span></span>|<span data-ttu-id="6e5a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e5a5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e5a5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="6e5a5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e5a5-118">Request headers</span></span>
|<span data-ttu-id="6e5a5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e5a5-119">Header</span></span>|<span data-ttu-id="6e5a5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6e5a5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e5a5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e5a5-121">Authorization</span></span>|<span data-ttu-id="6e5a5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e5a5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6e5a5-123">Accept</span></span>|<span data-ttu-id="6e5a5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e5a5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e5a5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e5a5-125">Request body</span></span>
<span data-ttu-id="6e5a5-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6e5a5-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6e5a5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e5a5-128">Property</span></span>|<span data-ttu-id="6e5a5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6e5a5-129">Type</span></span>|<span data-ttu-id="6e5a5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6e5a5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e5a5-131">priority</span><span class="sxs-lookup"><span data-stu-id="6e5a5-131">priority</span></span>|<span data-ttu-id="6e5a5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6e5a5-132">Int32</span></span>|<span data-ttu-id="6e5a5-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6e5a5-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e5a5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e5a5-134">Response</span></span>
<span data-ttu-id="6e5a5-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e5a5-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6e5a5-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e5a5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e5a5-137">Request</span></span>
<span data-ttu-id="6e5a5-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="6e5a5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e5a5-139">Response</span></span>
<span data-ttu-id="6e5a5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e5a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



