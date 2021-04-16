---
title: Действие setPriority
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b43942df6eb856b70d690532065a500f5d785bfb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864167"
---
# <a name="setpriority-action"></a><span data-ttu-id="2a141-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="2a141-103">setPriority action</span></span>

<span data-ttu-id="2a141-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a141-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a141-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a141-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a141-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a141-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a141-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2a141-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a141-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a141-108">Prerequisites</span></span>
<span data-ttu-id="2a141-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a141-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a141-111">Permission type</span></span>|<span data-ttu-id="2a141-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a141-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a141-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a141-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2a141-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2a141-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2a141-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a141-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a141-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a141-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a141-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a141-117">Not supported.</span></span>|
|<span data-ttu-id="2a141-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2a141-118">Application</span></span>||
| <span data-ttu-id="2a141-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2a141-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2a141-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a141-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a141-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a141-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="2a141-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a141-122">Request headers</span></span>
|<span data-ttu-id="2a141-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a141-123">Header</span></span>|<span data-ttu-id="2a141-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2a141-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a141-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a141-125">Authorization</span></span>|<span data-ttu-id="2a141-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a141-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a141-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2a141-127">Accept</span></span>|<span data-ttu-id="2a141-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2a141-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a141-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a141-129">Request body</span></span>
<span data-ttu-id="2a141-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a141-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2a141-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2a141-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2a141-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a141-132">Property</span></span>|<span data-ttu-id="2a141-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2a141-133">Type</span></span>|<span data-ttu-id="2a141-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2a141-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a141-135">priority</span><span class="sxs-lookup"><span data-stu-id="2a141-135">priority</span></span>|<span data-ttu-id="2a141-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2a141-136">Int32</span></span>|<span data-ttu-id="2a141-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2a141-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2a141-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a141-138">Response</span></span>
<span data-ttu-id="2a141-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2a141-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a141-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2a141-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a141-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a141-141">Request</span></span>
<span data-ttu-id="2a141-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a141-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="2a141-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a141-143">Response</span></span>
<span data-ttu-id="2a141-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a141-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







