---
title: Действие setPriority
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6021e05ee3a86d73386794e48059a5956384d23
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940014"
---
# <a name="setpriority-action"></a><span data-ttu-id="4d2fa-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="4d2fa-103">setPriority action</span></span>

> <span data-ttu-id="4d2fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d2fa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d2fa-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d2fa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d2fa-107">Prerequisites</span></span>
<span data-ttu-id="4d2fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2fa-110">Permission type</span></span>|<span data-ttu-id="4d2fa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d2fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d2fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d2fa-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4d2fa-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4d2fa-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4d2fa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2fa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d2fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d2fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d2fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-116">Not supported.</span></span>|
|<span data-ttu-id="4d2fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d2fa-117">Application</span></span>||
| <span data-ttu-id="4d2fa-118">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4d2fa-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4d2fa-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2fa-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d2fa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d2fa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="4d2fa-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4d2fa-121">Request headers</span></span>
|<span data-ttu-id="4d2fa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d2fa-122">Header</span></span>|<span data-ttu-id="4d2fa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4d2fa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d2fa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d2fa-124">Authorization</span></span>|<span data-ttu-id="4d2fa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d2fa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4d2fa-126">Accept</span></span>|<span data-ttu-id="4d2fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4d2fa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d2fa-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d2fa-128">Request body</span></span>
<span data-ttu-id="4d2fa-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d2fa-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d2fa-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d2fa-131">Property</span></span>|<span data-ttu-id="4d2fa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4d2fa-132">Type</span></span>|<span data-ttu-id="4d2fa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2fa-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d2fa-134">priority</span><span class="sxs-lookup"><span data-stu-id="4d2fa-134">priority</span></span>|<span data-ttu-id="4d2fa-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4d2fa-135">Int32</span></span>|<span data-ttu-id="4d2fa-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d2fa-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d2fa-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d2fa-137">Response</span></span>
<span data-ttu-id="4d2fa-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d2fa-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4d2fa-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d2fa-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2fa-140">Request</span></span>
<span data-ttu-id="4d2fa-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="4d2fa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2fa-142">Response</span></span>
<span data-ttu-id="4d2fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d2fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








