---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6841ed6e124ef0e30e60cded5b62682fcc94a298
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919654"
---
# <a name="delete-user"></a><span data-ttu-id="e3a53-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="e3a53-103">Delete user</span></span>

> <span data-ttu-id="e3a53-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3a53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3a53-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3a53-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3a53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3a53-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e3a53-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3a53-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3a53-108">Prerequisites</span></span>
<span data-ttu-id="e3a53-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e3a53-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e3a53-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a53-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e3a53-111">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="e3a53-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="e3a53-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a53-112">Permission type</span></span>|<span data-ttu-id="e3a53-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3a53-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3a53-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3a53-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3a53-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e3a53-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e3a53-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a53-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e3a53-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="e3a53-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e3a53-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a53-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e3a53-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="e3a53-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e3a53-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a53-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="e3a53-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="e3a53-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e3a53-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a53-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3a53-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3a53-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3a53-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a53-124">Not supported.</span></span>|
|<span data-ttu-id="e3a53-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3a53-125">Application</span></span>|<span data-ttu-id="e3a53-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a53-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3a53-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3a53-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="e3a53-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3a53-128">Request headers</span></span>

|<span data-ttu-id="e3a53-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3a53-129">Header</span></span>|<span data-ttu-id="e3a53-130">Значение</span><span class="sxs-lookup"><span data-stu-id="e3a53-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3a53-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a53-131">Authorization</span></span>|<span data-ttu-id="e3a53-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3a53-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3a53-133">Accept</span><span class="sxs-lookup"><span data-stu-id="e3a53-133">Accept</span></span>|<span data-ttu-id="e3a53-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e3a53-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3a53-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3a53-135">Request body</span></span>

<span data-ttu-id="e3a53-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3a53-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3a53-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a53-137">Response</span></span>

<span data-ttu-id="e3a53-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3a53-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3a53-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e3a53-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3a53-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a53-140">Request</span></span>

<span data-ttu-id="e3a53-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3a53-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="e3a53-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a53-142">Response</span></span>

<span data-ttu-id="e3a53-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3a53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



