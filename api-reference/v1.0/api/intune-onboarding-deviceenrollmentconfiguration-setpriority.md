---
title: Действие setPriority
description: Н/Д
author: tfitzmac
ms.openlocfilehash: d9d4eb0beb72187a71771148985466a5f72644a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303943"
---
# <a name="setpriority-action"></a><span data-ttu-id="2661e-103">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="2661e-103">setPriority action</span></span>

> <span data-ttu-id="2661e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2661e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2661e-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2661e-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2661e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2661e-106">Prerequisites</span></span>
<span data-ttu-id="2661e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2661e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2661e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2661e-109">Permission type</span></span>|<span data-ttu-id="2661e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2661e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2661e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2661e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2661e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2661e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2661e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2661e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2661e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2661e-114">Not supported.</span></span>|
|<span data-ttu-id="2661e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2661e-115">Application</span></span>|<span data-ttu-id="2661e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2661e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2661e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2661e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="2661e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2661e-118">Request headers</span></span>
|<span data-ttu-id="2661e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2661e-119">Header</span></span>|<span data-ttu-id="2661e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2661e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2661e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2661e-121">Authorization</span></span>|<span data-ttu-id="2661e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2661e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2661e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2661e-123">Accept</span></span>|<span data-ttu-id="2661e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2661e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2661e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2661e-125">Request body</span></span>
<span data-ttu-id="2661e-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2661e-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2661e-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2661e-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2661e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2661e-128">Property</span></span>|<span data-ttu-id="2661e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2661e-129">Type</span></span>|<span data-ttu-id="2661e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2661e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2661e-131">priority</span><span class="sxs-lookup"><span data-stu-id="2661e-131">priority</span></span>|<span data-ttu-id="2661e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2661e-132">Int32</span></span>|<span data-ttu-id="2661e-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2661e-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2661e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2661e-134">Response</span></span>
<span data-ttu-id="2661e-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2661e-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2661e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2661e-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="2661e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2661e-137">Request</span></span>
<span data-ttu-id="2661e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2661e-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="2661e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2661e-139">Response</span></span>
<span data-ttu-id="2661e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2661e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



