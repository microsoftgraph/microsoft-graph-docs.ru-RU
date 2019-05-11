---
title: Действие wipeManagedAppRegistrationByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05935def6d23c18726622037b52e5586a06925f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33897865"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="9fb19-103">Действие wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="9fb19-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="9fb19-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9fb19-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9fb19-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fb19-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fb19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fb19-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="9fb19-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fb19-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9fb19-108">Prerequisites</span></span>

<span data-ttu-id="9fb19-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fb19-111">Permission type</span></span>|<span data-ttu-id="9fb19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fb19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fb19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fb19-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9fb19-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="9fb19-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="9fb19-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb19-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fb19-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fb19-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fb19-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb19-117">Not supported.</span></span>|
|<span data-ttu-id="9fb19-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fb19-118">Application</span></span>|<span data-ttu-id="9fb19-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb19-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fb19-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fb19-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="9fb19-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fb19-121">Request headers</span></span>

|<span data-ttu-id="9fb19-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fb19-122">Header</span></span>|<span data-ttu-id="9fb19-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9fb19-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fb19-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fb19-124">Authorization</span></span>|<span data-ttu-id="9fb19-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fb19-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fb19-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9fb19-126">Accept</span></span>|<span data-ttu-id="9fb19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9fb19-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fb19-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fb19-128">Request body</span></span>

<span data-ttu-id="9fb19-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fb19-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9fb19-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9fb19-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9fb19-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fb19-131">Property</span></span>|<span data-ttu-id="9fb19-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9fb19-132">Type</span></span>|<span data-ttu-id="9fb19-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb19-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb19-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9fb19-134">deviceTag</span></span>|<span data-ttu-id="9fb19-135">String</span><span class="sxs-lookup"><span data-stu-id="9fb19-135">String</span></span>|<span data-ttu-id="9fb19-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="9fb19-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="9fb19-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb19-137">Response</span></span>

<span data-ttu-id="9fb19-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9fb19-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9fb19-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9fb19-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fb19-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fb19-140">Request</span></span>

<span data-ttu-id="9fb19-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fb19-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="9fb19-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb19-142">Response</span></span>

<span data-ttu-id="9fb19-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fb19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






