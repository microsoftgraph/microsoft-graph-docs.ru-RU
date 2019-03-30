---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecf07bf080a76e6f1fce515d41090be214e7a514
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986637"
---
# <a name="delete-user"></a><span data-ttu-id="11b8a-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="11b8a-103">Delete user</span></span>

> <span data-ttu-id="11b8a-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11b8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11b8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11b8a-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11b8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b8a-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="11b8a-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11b8a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11b8a-108">Prerequisites</span></span>
<span data-ttu-id="11b8a-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="11b8a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="11b8a-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b8a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="11b8a-111">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="11b8a-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="11b8a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b8a-112">Permission type</span></span>|<span data-ttu-id="11b8a-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b8a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11b8a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b8a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="11b8a-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="11b8a-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="11b8a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b8a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="11b8a-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="11b8a-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="11b8a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b8a-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="11b8a-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="11b8a-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="11b8a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b8a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="11b8a-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="11b8a-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="11b8a-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b8a-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="11b8a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b8a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11b8a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b8a-124">Not supported.</span></span>|
|<span data-ttu-id="11b8a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11b8a-125">Application</span></span>|<span data-ttu-id="11b8a-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b8a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11b8a-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b8a-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="11b8a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11b8a-128">Request headers</span></span>

|<span data-ttu-id="11b8a-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11b8a-129">Header</span></span>|<span data-ttu-id="11b8a-130">Значение</span><span class="sxs-lookup"><span data-stu-id="11b8a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11b8a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11b8a-131">Authorization</span></span>|<span data-ttu-id="11b8a-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b8a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11b8a-133">Accept</span><span class="sxs-lookup"><span data-stu-id="11b8a-133">Accept</span></span>|<span data-ttu-id="11b8a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="11b8a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b8a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11b8a-135">Request body</span></span>

<span data-ttu-id="11b8a-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11b8a-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11b8a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="11b8a-137">Response</span></span>

<span data-ttu-id="11b8a-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="11b8a-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11b8a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="11b8a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="11b8a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b8a-140">Request</span></span>

<span data-ttu-id="11b8a-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11b8a-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="11b8a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b8a-142">Response</span></span>

<span data-ttu-id="11b8a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11b8a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



