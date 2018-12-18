---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
ms.openlocfilehash: c08ba0bb670b2429cd97f7a23a8790ccc6c5c487
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318972"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="d8815-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="d8815-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="d8815-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8815-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8815-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8815-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8815-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8815-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8815-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="d8815-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8815-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8815-108">Prerequisites</span></span>

<span data-ttu-id="d8815-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8815-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8815-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8815-111">Permission type</span></span>|<span data-ttu-id="d8815-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8815-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8815-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8815-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8815-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d8815-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d8815-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8815-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8815-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8815-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8815-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8815-117">Not supported.</span></span>|
|<span data-ttu-id="d8815-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8815-118">Application</span></span>|<span data-ttu-id="d8815-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8815-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8815-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8815-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="d8815-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8815-121">Request headers</span></span>

|<span data-ttu-id="d8815-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8815-122">Header</span></span>|<span data-ttu-id="d8815-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d8815-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8815-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8815-124">Authorization</span></span>|<span data-ttu-id="d8815-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8815-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8815-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d8815-126">Accept</span></span>|<span data-ttu-id="d8815-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8815-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8815-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8815-128">Request body</span></span>

<span data-ttu-id="d8815-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8815-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d8815-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d8815-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d8815-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8815-131">Property</span></span>|<span data-ttu-id="d8815-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d8815-132">Type</span></span>|<span data-ttu-id="d8815-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d8815-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8815-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d8815-134">deviceTag</span></span>|<span data-ttu-id="d8815-135">String</span><span class="sxs-lookup"><span data-stu-id="d8815-135">String</span></span>|<span data-ttu-id="d8815-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="d8815-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="d8815-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8815-137">Response</span></span>

<span data-ttu-id="d8815-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d8815-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d8815-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d8815-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8815-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8815-140">Request</span></span>

<span data-ttu-id="d8815-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8815-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="d8815-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8815-142">Response</span></span>

<span data-ttu-id="d8815-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8815-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






