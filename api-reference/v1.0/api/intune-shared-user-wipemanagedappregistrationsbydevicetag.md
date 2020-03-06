---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 414cad053f4f48267737b608a57f14a3df8f5c8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511945"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="6e107-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="6e107-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="6e107-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e107-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e107-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e107-106">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="6e107-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e107-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6e107-107">Prerequisites</span></span>
<span data-ttu-id="6e107-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e107-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e107-110">Permission type</span></span>|<span data-ttu-id="6e107-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e107-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e107-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6e107-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="6e107-113">_varies by context_</span></span> |
| <span data-ttu-id="6e107-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="6e107-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="6e107-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e107-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="6e107-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e107-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e107-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e107-117">Not supported.</span></span>|
|<span data-ttu-id="6e107-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e107-118">Application</span></span>|<span data-ttu-id="6e107-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e107-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e107-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e107-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="6e107-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e107-121">Request headers</span></span>
|<span data-ttu-id="6e107-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e107-122">Header</span></span>|<span data-ttu-id="6e107-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6e107-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e107-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e107-124">Authorization</span></span>|<span data-ttu-id="6e107-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e107-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e107-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6e107-126">Accept</span></span>|<span data-ttu-id="6e107-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6e107-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e107-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e107-128">Request body</span></span>
<span data-ttu-id="6e107-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e107-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6e107-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6e107-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6e107-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e107-131">Property</span></span>|<span data-ttu-id="6e107-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6e107-132">Type</span></span>|<span data-ttu-id="6e107-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6e107-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e107-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6e107-134">deviceTag</span></span>|<span data-ttu-id="6e107-135">String</span><span class="sxs-lookup"><span data-stu-id="6e107-135">String</span></span>|<span data-ttu-id="6e107-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="6e107-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="6e107-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e107-137">Response</span></span>
<span data-ttu-id="6e107-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6e107-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e107-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6e107-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e107-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e107-140">Request</span></span>
<span data-ttu-id="6e107-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e107-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="6e107-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e107-142">Response</span></span>
<span data-ttu-id="6e107-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e107-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




