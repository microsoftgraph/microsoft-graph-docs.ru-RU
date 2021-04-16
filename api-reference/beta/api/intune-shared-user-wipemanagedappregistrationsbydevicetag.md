---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf8cd20fd822f7fb95f763775c8b693dddcc1267
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865028"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="902fa-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="902fa-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="902fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="902fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="902fa-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="902fa-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="902fa-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902fa-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="902fa-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="902fa-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="902fa-108">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="902fa-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="902fa-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="902fa-109">Prerequisites</span></span>

<span data-ttu-id="902fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902fa-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="902fa-112">Permission type</span></span>|<span data-ttu-id="902fa-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="902fa-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="902fa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="902fa-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="902fa-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="902fa-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="902fa-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902fa-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="902fa-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="902fa-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="902fa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902fa-118">Not supported.</span></span>|
|<span data-ttu-id="902fa-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="902fa-119">Application</span></span>||
| <span data-ttu-id="902fa-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="902fa-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="902fa-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902fa-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="902fa-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="902fa-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="902fa-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="902fa-123">Request headers</span></span>

|<span data-ttu-id="902fa-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="902fa-124">Header</span></span>|<span data-ttu-id="902fa-125">Значение</span><span class="sxs-lookup"><span data-stu-id="902fa-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="902fa-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="902fa-126">Authorization</span></span>|<span data-ttu-id="902fa-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="902fa-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="902fa-128">Accept</span><span class="sxs-lookup"><span data-stu-id="902fa-128">Accept</span></span>|<span data-ttu-id="902fa-129">application/json</span><span class="sxs-lookup"><span data-stu-id="902fa-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="902fa-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="902fa-130">Request body</span></span>

<span data-ttu-id="902fa-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902fa-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="902fa-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="902fa-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="902fa-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="902fa-133">Property</span></span>|<span data-ttu-id="902fa-134">Тип</span><span class="sxs-lookup"><span data-stu-id="902fa-134">Type</span></span>|<span data-ttu-id="902fa-135">Описание</span><span class="sxs-lookup"><span data-stu-id="902fa-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="902fa-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="902fa-136">deviceTag</span></span>|<span data-ttu-id="902fa-137">String</span><span class="sxs-lookup"><span data-stu-id="902fa-137">String</span></span>|<span data-ttu-id="902fa-138">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="902fa-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="902fa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="902fa-139">Response</span></span>

<span data-ttu-id="902fa-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="902fa-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="902fa-141">Пример</span><span class="sxs-lookup"><span data-stu-id="902fa-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="902fa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="902fa-142">Request</span></span>

<span data-ttu-id="902fa-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="902fa-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="902fa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="902fa-144">Response</span></span>

<span data-ttu-id="902fa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="902fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```













