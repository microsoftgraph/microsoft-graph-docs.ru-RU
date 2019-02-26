---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4d74df507e3172713fea4179b321fdf05cc06be
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261154"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="c55c8-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="c55c8-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="c55c8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c55c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c55c8-105">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="c55c8-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c55c8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c55c8-106">Prerequisites</span></span>
<span data-ttu-id="c55c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c55c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c55c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c55c8-109">Permission type</span></span>|<span data-ttu-id="c55c8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c55c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c55c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c55c8-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c55c8-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="c55c8-112">_varies by context_</span></span> |
| <span data-ttu-id="c55c8-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c55c8-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c55c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55c8-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="c55c8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c55c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c55c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c55c8-116">Not supported.</span></span>|
|<span data-ttu-id="c55c8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c55c8-117">Application</span></span>|<span data-ttu-id="c55c8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c55c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c55c8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c55c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="c55c8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c55c8-120">Request headers</span></span>
|<span data-ttu-id="c55c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c55c8-121">Header</span></span>|<span data-ttu-id="c55c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c55c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c55c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c55c8-123">Authorization</span></span>|<span data-ttu-id="c55c8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c55c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c55c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c55c8-125">Accept</span></span>|<span data-ttu-id="c55c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c55c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c55c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c55c8-127">Request body</span></span>
<span data-ttu-id="c55c8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c55c8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c55c8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c55c8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c55c8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c55c8-130">Property</span></span>|<span data-ttu-id="c55c8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c55c8-131">Type</span></span>|<span data-ttu-id="c55c8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c55c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c55c8-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c55c8-133">deviceTag</span></span>|<span data-ttu-id="c55c8-134">String</span><span class="sxs-lookup"><span data-stu-id="c55c8-134">String</span></span>|<span data-ttu-id="c55c8-135">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="c55c8-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="c55c8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c55c8-136">Response</span></span>
<span data-ttu-id="c55c8-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c55c8-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c55c8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c55c8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c55c8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c55c8-139">Request</span></span>
<span data-ttu-id="c55c8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c55c8-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="c55c8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c55c8-141">Response</span></span>
<span data-ttu-id="c55c8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c55c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



