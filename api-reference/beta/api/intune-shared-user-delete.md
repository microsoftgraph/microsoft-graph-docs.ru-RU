---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
ms.openlocfilehash: 950e267a929bc1c04627e94207bc933bff4466cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309438"
---
# <a name="delete-user"></a><span data-ttu-id="2a543-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="2a543-103">Delete user</span></span>

> <span data-ttu-id="2a543-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2a543-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a543-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a543-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a543-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a543-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a543-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="2a543-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a543-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a543-108">Prerequisites</span></span>
<span data-ttu-id="2a543-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2a543-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2a543-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a543-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="2a543-111">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="2a543-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="2a543-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a543-112">Permission type</span></span>|<span data-ttu-id="2a543-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a543-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a543-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a543-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2a543-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2a543-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2a543-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a543-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2a543-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="2a543-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2a543-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a543-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2a543-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="2a543-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2a543-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a543-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="2a543-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="2a543-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2a543-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a543-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2a543-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a543-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a543-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a543-124">Not supported.</span></span>|
|<span data-ttu-id="2a543-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a543-125">Application</span></span>|<span data-ttu-id="2a543-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a543-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a543-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a543-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="2a543-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a543-128">Request headers</span></span>

|<span data-ttu-id="2a543-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a543-129">Header</span></span>|<span data-ttu-id="2a543-130">Значение</span><span class="sxs-lookup"><span data-stu-id="2a543-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a543-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a543-131">Authorization</span></span>|<span data-ttu-id="2a543-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2a543-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a543-133">Accept</span><span class="sxs-lookup"><span data-stu-id="2a543-133">Accept</span></span>|<span data-ttu-id="2a543-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2a543-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a543-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a543-135">Request body</span></span>

<span data-ttu-id="2a543-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a543-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a543-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a543-137">Response</span></span>

<span data-ttu-id="2a543-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2a543-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a543-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2a543-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a543-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a543-140">Request</span></span>

<span data-ttu-id="2a543-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a543-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="2a543-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a543-142">Response</span></span>

<span data-ttu-id="2a543-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2a543-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



