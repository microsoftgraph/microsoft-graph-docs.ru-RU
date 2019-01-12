---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 80e7b83001cf177cacaeb84d814509f31cd340cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972007"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="00ccc-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="00ccc-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="00ccc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00ccc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00ccc-105">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="00ccc-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00ccc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00ccc-106">Prerequisites</span></span>
<span data-ttu-id="00ccc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ccc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00ccc-109">Permission type</span></span>|<span data-ttu-id="00ccc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00ccc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00ccc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00ccc-111">Delegated (work or school account)</span></span>| <span data-ttu-id="00ccc-112">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="00ccc-112">_varies by context_</span></span> |
| <span data-ttu-id="00ccc-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="00ccc-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="00ccc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ccc-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="00ccc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00ccc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00ccc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ccc-116">Not supported.</span></span>|
|<span data-ttu-id="00ccc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00ccc-117">Application</span></span>|<span data-ttu-id="00ccc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ccc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00ccc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00ccc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="00ccc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00ccc-120">Request headers</span></span>
|<span data-ttu-id="00ccc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00ccc-121">Header</span></span>|<span data-ttu-id="00ccc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00ccc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00ccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ccc-123">Authorization</span></span>|<span data-ttu-id="00ccc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00ccc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00ccc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00ccc-125">Accept</span></span>|<span data-ttu-id="00ccc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00ccc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ccc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00ccc-127">Request body</span></span>
<span data-ttu-id="00ccc-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00ccc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="00ccc-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="00ccc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="00ccc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00ccc-130">Property</span></span>|<span data-ttu-id="00ccc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00ccc-131">Type</span></span>|<span data-ttu-id="00ccc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00ccc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ccc-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="00ccc-133">deviceTag</span></span>|<span data-ttu-id="00ccc-134">String</span><span class="sxs-lookup"><span data-stu-id="00ccc-134">String</span></span>|<span data-ttu-id="00ccc-135">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="00ccc-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="00ccc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ccc-136">Response</span></span>
<span data-ttu-id="00ccc-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="00ccc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="00ccc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="00ccc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="00ccc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ccc-139">Request</span></span>
<span data-ttu-id="00ccc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00ccc-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="00ccc-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="00ccc-141">Response</span></span>
<span data-ttu-id="00ccc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00ccc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



