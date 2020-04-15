---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 473c57670a026e538585e98338d202238428a1b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411213"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="2e7b2-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="2e7b2-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="2e7b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e7b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e7b2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e7b2-106">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e7b2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e7b2-107">Prerequisites</span></span>
<span data-ttu-id="2e7b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e7b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e7b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e7b2-110">Permission type</span></span>|<span data-ttu-id="2e7b2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e7b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e7b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e7b2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2e7b2-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="2e7b2-113">_varies by context_</span></span> |
| <span data-ttu-id="2e7b2-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="2e7b2-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="2e7b2-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e7b2-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="2e7b2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e7b2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e7b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-117">Not supported.</span></span>|
|<span data-ttu-id="2e7b2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e7b2-118">Application</span></span>|<span data-ttu-id="2e7b2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e7b2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e7b2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="2e7b2-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e7b2-121">Request headers</span></span>
|<span data-ttu-id="2e7b2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e7b2-122">Header</span></span>|<span data-ttu-id="2e7b2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2e7b2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e7b2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e7b2-124">Authorization</span></span>|<span data-ttu-id="2e7b2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e7b2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2e7b2-126">Accept</span></span>|<span data-ttu-id="2e7b2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2e7b2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e7b2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e7b2-128">Request body</span></span>
<span data-ttu-id="2e7b2-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2e7b2-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2e7b2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e7b2-131">Property</span></span>|<span data-ttu-id="2e7b2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2e7b2-132">Type</span></span>|<span data-ttu-id="2e7b2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2e7b2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7b2-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="2e7b2-134">deviceTag</span></span>|<span data-ttu-id="2e7b2-135">String</span><span class="sxs-lookup"><span data-stu-id="2e7b2-135">String</span></span>|<span data-ttu-id="2e7b2-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="2e7b2-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="2e7b2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e7b2-137">Response</span></span>
<span data-ttu-id="2e7b2-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e7b2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2e7b2-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e7b2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e7b2-140">Request</span></span>
<span data-ttu-id="2e7b2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="2e7b2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e7b2-142">Response</span></span>
<span data-ttu-id="2e7b2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e7b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






