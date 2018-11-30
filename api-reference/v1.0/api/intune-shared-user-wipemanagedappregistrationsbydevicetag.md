---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
ms.openlocfilehash: d6f56fa50b3162ecaebc0bb1adb02af3b4b0e9f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026946"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="559c9-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="559c9-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="559c9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="559c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="559c9-105">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="559c9-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="559c9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="559c9-106">Prerequisites</span></span>
<span data-ttu-id="559c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="559c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="559c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="559c9-109">Permission type</span></span>|<span data-ttu-id="559c9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="559c9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="559c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="559c9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="559c9-112">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="559c9-112">_varies by context_</span></span> |
| <span data-ttu-id="559c9-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="559c9-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="559c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="559c9-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="559c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="559c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="559c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="559c9-116">Not supported.</span></span>|
|<span data-ttu-id="559c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="559c9-117">Application</span></span>|<span data-ttu-id="559c9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="559c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="559c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="559c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="559c9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="559c9-120">Request headers</span></span>
|<span data-ttu-id="559c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="559c9-121">Header</span></span>|<span data-ttu-id="559c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="559c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="559c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="559c9-123">Authorization</span></span>|<span data-ttu-id="559c9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="559c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="559c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="559c9-125">Accept</span></span>|<span data-ttu-id="559c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="559c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="559c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="559c9-127">Request body</span></span>
<span data-ttu-id="559c9-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="559c9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="559c9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="559c9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="559c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="559c9-130">Property</span></span>|<span data-ttu-id="559c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="559c9-131">Type</span></span>|<span data-ttu-id="559c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="559c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="559c9-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="559c9-133">deviceTag</span></span>|<span data-ttu-id="559c9-134">String</span><span class="sxs-lookup"><span data-stu-id="559c9-134">String</span></span>|<span data-ttu-id="559c9-135">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="559c9-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="559c9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="559c9-136">Response</span></span>
<span data-ttu-id="559c9-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="559c9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="559c9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="559c9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="559c9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="559c9-139">Request</span></span>
<span data-ttu-id="559c9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="559c9-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="559c9-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="559c9-141">Response</span></span>
<span data-ttu-id="559c9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="559c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



