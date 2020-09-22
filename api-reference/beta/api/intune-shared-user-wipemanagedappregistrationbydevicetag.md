---
title: Действие wipeManagedAppRegistrationByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e401b453907aeed9b700d2a79ac348bf961c7619
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085558"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="6feb3-103">Действие wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="6feb3-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

<span data-ttu-id="6feb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6feb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6feb3-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6feb3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6feb3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6feb3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6feb3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6feb3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6feb3-108">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="6feb3-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6feb3-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6feb3-109">Prerequisites</span></span>

<span data-ttu-id="6feb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6feb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6feb3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6feb3-112">Permission type</span></span>|<span data-ttu-id="6feb3-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6feb3-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6feb3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6feb3-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6feb3-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="6feb3-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6feb3-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6feb3-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6feb3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6feb3-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6feb3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6feb3-118">Not supported.</span></span>|
|<span data-ttu-id="6feb3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6feb3-119">Application</span></span>||
| <span data-ttu-id="6feb3-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="6feb3-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6feb3-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6feb3-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6feb3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6feb3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="6feb3-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6feb3-123">Request headers</span></span>

|<span data-ttu-id="6feb3-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6feb3-124">Header</span></span>|<span data-ttu-id="6feb3-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6feb3-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6feb3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6feb3-126">Authorization</span></span>|<span data-ttu-id="6feb3-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6feb3-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6feb3-128">Accept</span><span class="sxs-lookup"><span data-stu-id="6feb3-128">Accept</span></span>|<span data-ttu-id="6feb3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6feb3-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6feb3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6feb3-130">Request body</span></span>

<span data-ttu-id="6feb3-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6feb3-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6feb3-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6feb3-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6feb3-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6feb3-133">Property</span></span>|<span data-ttu-id="6feb3-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6feb3-134">Type</span></span>|<span data-ttu-id="6feb3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6feb3-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6feb3-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6feb3-136">deviceTag</span></span>|<span data-ttu-id="6feb3-137">String</span><span class="sxs-lookup"><span data-stu-id="6feb3-137">String</span></span>|<span data-ttu-id="6feb3-138">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="6feb3-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="6feb3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6feb3-139">Response</span></span>

<span data-ttu-id="6feb3-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6feb3-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6feb3-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6feb3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6feb3-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6feb3-142">Request</span></span>

<span data-ttu-id="6feb3-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6feb3-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="6feb3-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6feb3-144">Response</span></span>

<span data-ttu-id="6feb3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6feb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```















