---
title: Удаление пользователя
description: Удаляет объект user.
ms.openlocfilehash: 3b580e46fe15e81e0325f9b673217e41274b8721
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026998"
---
# <a name="delete-user"></a><span data-ttu-id="5f1f6-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="5f1f6-103">Delete user</span></span>

> <span data-ttu-id="5f1f6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f1f6-105">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f1f6-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f1f6-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f1f6-106">Prerequisites</span></span>
<span data-ttu-id="5f1f6-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5f1f6-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1f6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="5f1f6-109">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="5f1f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f1f6-110">Permission type</span></span>|<span data-ttu-id="5f1f6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f1f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5f1f6-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="5f1f6-113">_varies by context_</span></span>|
| <span data-ttu-id="5f1f6-114">&nbsp;&nbsp; Устройств</span><span class="sxs-lookup"><span data-stu-id="5f1f6-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="5f1f6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5f1f6-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5f1f6-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="5f1f6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5f1f6-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="5f1f6-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5f1f6-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5f1f6-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5f1f6-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5f1f6-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="5f1f6-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f1f6-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-123">Not supported.</span></span>|
|<span data-ttu-id="5f1f6-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f1f6-124">Application</span></span>|<span data-ttu-id="5f1f6-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f1f6-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f1f6-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="5f1f6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f1f6-127">Request headers</span></span>
|<span data-ttu-id="5f1f6-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f1f6-128">Header</span></span>|<span data-ttu-id="5f1f6-129">Значение</span><span class="sxs-lookup"><span data-stu-id="5f1f6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f1f6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f1f6-130">Authorization</span></span>|<span data-ttu-id="5f1f6-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5f1f6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f1f6-132">Accept</span><span class="sxs-lookup"><span data-stu-id="5f1f6-132">Accept</span></span>|<span data-ttu-id="5f1f6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5f1f6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f1f6-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f1f6-134">Request body</span></span>
<span data-ttu-id="5f1f6-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f1f6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f1f6-136">Response</span></span>
<span data-ttu-id="5f1f6-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f1f6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5f1f6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f1f6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f1f6-139">Request</span></span>
<span data-ttu-id="5f1f6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="5f1f6-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f1f6-141">Response</span></span>
<span data-ttu-id="5f1f6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5f1f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



