---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20f58ba0731f97c81220150e06250be0cdd31173
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194346"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="852f3-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="852f3-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="852f3-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="852f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="852f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="852f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="852f3-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="852f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="852f3-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="852f3-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="852f3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="852f3-108">Prerequisites</span></span>

<span data-ttu-id="852f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="852f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="852f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="852f3-111">Permission type</span></span>|<span data-ttu-id="852f3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="852f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="852f3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="852f3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="852f3-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="852f3-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="852f3-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852f3-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="852f3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="852f3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="852f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="852f3-117">Not supported.</span></span>|
|<span data-ttu-id="852f3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="852f3-118">Application</span></span>||
| <span data-ttu-id="852f3-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="852f3-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="852f3-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852f3-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="852f3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="852f3-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="852f3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="852f3-122">Request headers</span></span>

|<span data-ttu-id="852f3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="852f3-123">Header</span></span>|<span data-ttu-id="852f3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="852f3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="852f3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="852f3-125">Authorization</span></span>|<span data-ttu-id="852f3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="852f3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="852f3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="852f3-127">Accept</span></span>|<span data-ttu-id="852f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="852f3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="852f3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="852f3-129">Request body</span></span>

<span data-ttu-id="852f3-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="852f3-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="852f3-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="852f3-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="852f3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="852f3-132">Property</span></span>|<span data-ttu-id="852f3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="852f3-133">Type</span></span>|<span data-ttu-id="852f3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="852f3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="852f3-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="852f3-135">deviceTag</span></span>|<span data-ttu-id="852f3-136">String</span><span class="sxs-lookup"><span data-stu-id="852f3-136">String</span></span>|<span data-ttu-id="852f3-137">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="852f3-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="852f3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="852f3-138">Response</span></span>

<span data-ttu-id="852f3-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="852f3-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="852f3-140">Пример</span><span class="sxs-lookup"><span data-stu-id="852f3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="852f3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="852f3-141">Request</span></span>

<span data-ttu-id="852f3-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="852f3-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="852f3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="852f3-143">Response</span></span>

<span data-ttu-id="852f3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="852f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










