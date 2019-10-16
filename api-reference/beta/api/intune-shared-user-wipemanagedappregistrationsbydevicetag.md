---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c19e42e767321a4e0041c054cea3adf06b40478
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537869"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="3d9d9-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="3d9d9-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="3d9d9-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d9d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d9d9-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d9d9-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d9d9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3d9d9-108">Prerequisites</span></span>

<span data-ttu-id="3d9d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d9d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d9d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d9d9-111">Permission type</span></span>|<span data-ttu-id="3d9d9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d9d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d9d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d9d9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3d9d9-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3d9d9-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9d9-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d9d9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d9d9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d9d9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-117">Not supported.</span></span>|
|<span data-ttu-id="3d9d9-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d9d9-118">Application</span></span>||
| <span data-ttu-id="3d9d9-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3d9d9-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9d9-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d9d9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d9d9-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="3d9d9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d9d9-122">Request headers</span></span>

|<span data-ttu-id="3d9d9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d9d9-123">Header</span></span>|<span data-ttu-id="3d9d9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3d9d9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d9d9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d9d9-125">Authorization</span></span>|<span data-ttu-id="3d9d9-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d9d9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3d9d9-127">Accept</span></span>|<span data-ttu-id="3d9d9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3d9d9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d9d9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d9d9-129">Request body</span></span>

<span data-ttu-id="3d9d9-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3d9d9-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3d9d9-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d9d9-132">Property</span></span>|<span data-ttu-id="3d9d9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3d9d9-133">Type</span></span>|<span data-ttu-id="3d9d9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3d9d9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d9d9-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3d9d9-135">deviceTag</span></span>|<span data-ttu-id="3d9d9-136">String</span><span class="sxs-lookup"><span data-stu-id="3d9d9-136">String</span></span>|<span data-ttu-id="3d9d9-137">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="3d9d9-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="3d9d9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d9d9-138">Response</span></span>

<span data-ttu-id="3d9d9-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d9d9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3d9d9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d9d9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d9d9-141">Request</span></span>

<span data-ttu-id="3d9d9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="3d9d9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d9d9-143">Response</span></span>

<span data-ttu-id="3d9d9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












