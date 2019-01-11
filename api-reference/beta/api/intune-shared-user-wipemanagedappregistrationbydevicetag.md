---
title: Действие wipeManagedAppRegistrationByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68d3e2d2a356e23c4b83509c827aee4e18f72aac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821842"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="b0abb-103">Действие wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="b0abb-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="b0abb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0abb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0abb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0abb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0abb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b0abb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0abb-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="b0abb-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0abb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0abb-108">Prerequisites</span></span>

<span data-ttu-id="b0abb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0abb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0abb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0abb-111">Permission type</span></span>|<span data-ttu-id="b0abb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0abb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0abb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0abb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b0abb-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="b0abb-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="b0abb-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0abb-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0abb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0abb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0abb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0abb-117">Not supported.</span></span>|
|<span data-ttu-id="b0abb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0abb-118">Application</span></span>|<span data-ttu-id="b0abb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0abb-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0abb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0abb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="b0abb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0abb-121">Request headers</span></span>

|<span data-ttu-id="b0abb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0abb-122">Header</span></span>|<span data-ttu-id="b0abb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b0abb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0abb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0abb-124">Authorization</span></span>|<span data-ttu-id="b0abb-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b0abb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0abb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b0abb-126">Accept</span></span>|<span data-ttu-id="b0abb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0abb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0abb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0abb-128">Request body</span></span>

<span data-ttu-id="b0abb-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0abb-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b0abb-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b0abb-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b0abb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0abb-131">Property</span></span>|<span data-ttu-id="b0abb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b0abb-132">Type</span></span>|<span data-ttu-id="b0abb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b0abb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0abb-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b0abb-134">deviceTag</span></span>|<span data-ttu-id="b0abb-135">String</span><span class="sxs-lookup"><span data-stu-id="b0abb-135">String</span></span>|<span data-ttu-id="b0abb-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="b0abb-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="b0abb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0abb-137">Response</span></span>

<span data-ttu-id="b0abb-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0abb-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0abb-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b0abb-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0abb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0abb-140">Request</span></span>

<span data-ttu-id="b0abb-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0abb-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="b0abb-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0abb-142">Response</span></span>

<span data-ttu-id="b0abb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0abb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






