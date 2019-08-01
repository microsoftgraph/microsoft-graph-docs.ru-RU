---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bea86526d1c8770ac1800442d5e0f2e06318fb58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025724"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="c37f2-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="c37f2-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="c37f2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c37f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c37f2-105">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="c37f2-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c37f2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c37f2-106">Prerequisites</span></span>
<span data-ttu-id="c37f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c37f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c37f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c37f2-109">Permission type</span></span>|<span data-ttu-id="c37f2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c37f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c37f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c37f2-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c37f2-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="c37f2-112">_varies by context_</span></span> |
| <span data-ttu-id="c37f2-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c37f2-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c37f2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37f2-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="c37f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c37f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c37f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c37f2-116">Not supported.</span></span>|
|<span data-ttu-id="c37f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c37f2-117">Application</span></span>|<span data-ttu-id="c37f2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c37f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c37f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c37f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="c37f2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c37f2-120">Request headers</span></span>
|<span data-ttu-id="c37f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c37f2-121">Header</span></span>|<span data-ttu-id="c37f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c37f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c37f2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c37f2-123">Authorization</span></span>|<span data-ttu-id="c37f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c37f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c37f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c37f2-125">Accept</span></span>|<span data-ttu-id="c37f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c37f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c37f2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c37f2-127">Request body</span></span>
<span data-ttu-id="c37f2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c37f2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c37f2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c37f2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c37f2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c37f2-130">Property</span></span>|<span data-ttu-id="c37f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c37f2-131">Type</span></span>|<span data-ttu-id="c37f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c37f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37f2-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c37f2-133">deviceTag</span></span>|<span data-ttu-id="c37f2-134">String</span><span class="sxs-lookup"><span data-stu-id="c37f2-134">String</span></span>|<span data-ttu-id="c37f2-135">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="c37f2-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="c37f2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37f2-136">Response</span></span>
<span data-ttu-id="c37f2-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c37f2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c37f2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c37f2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c37f2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c37f2-139">Request</span></span>
<span data-ttu-id="c37f2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c37f2-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="c37f2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37f2-141">Response</span></span>
<span data-ttu-id="c37f2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c37f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



