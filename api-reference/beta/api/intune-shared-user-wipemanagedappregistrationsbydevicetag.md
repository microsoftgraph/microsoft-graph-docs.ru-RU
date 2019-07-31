---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf4c11edbd0743c3ef4e641496cfb851e347b995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984085"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="77d0f-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="77d0f-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="77d0f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77d0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77d0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77d0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77d0f-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77d0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d0f-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="77d0f-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77d0f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77d0f-108">Prerequisites</span></span>

<span data-ttu-id="77d0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77d0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77d0f-111">Permission type</span></span>|<span data-ttu-id="77d0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77d0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77d0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77d0f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="77d0f-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="77d0f-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="77d0f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d0f-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77d0f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77d0f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77d0f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77d0f-117">Not supported.</span></span>|
|<span data-ttu-id="77d0f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77d0f-118">Application</span></span>|<span data-ttu-id="77d0f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77d0f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77d0f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77d0f-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="77d0f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77d0f-121">Request headers</span></span>

|<span data-ttu-id="77d0f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77d0f-122">Header</span></span>|<span data-ttu-id="77d0f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="77d0f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77d0f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77d0f-124">Authorization</span></span>|<span data-ttu-id="77d0f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77d0f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77d0f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="77d0f-126">Accept</span></span>|<span data-ttu-id="77d0f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="77d0f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77d0f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77d0f-128">Request body</span></span>

<span data-ttu-id="77d0f-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77d0f-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="77d0f-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="77d0f-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="77d0f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="77d0f-131">Property</span></span>|<span data-ttu-id="77d0f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="77d0f-132">Type</span></span>|<span data-ttu-id="77d0f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="77d0f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77d0f-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="77d0f-134">deviceTag</span></span>|<span data-ttu-id="77d0f-135">String</span><span class="sxs-lookup"><span data-stu-id="77d0f-135">String</span></span>|<span data-ttu-id="77d0f-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="77d0f-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="77d0f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="77d0f-137">Response</span></span>

<span data-ttu-id="77d0f-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="77d0f-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="77d0f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="77d0f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="77d0f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="77d0f-140">Request</span></span>

<span data-ttu-id="77d0f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77d0f-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="77d0f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="77d0f-142">Response</span></span>

<span data-ttu-id="77d0f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77d0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






