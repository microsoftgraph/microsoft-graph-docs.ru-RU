---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e389eb6fb871cc1a6d827b25e40332066657383d
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732932"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="45200-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="45200-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="45200-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45200-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45200-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45200-106">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="45200-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45200-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45200-107">Prerequisites</span></span>
<span data-ttu-id="45200-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45200-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45200-110">Permission type</span></span>|<span data-ttu-id="45200-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45200-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45200-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45200-112">Delegated (work or school account)</span></span>| <span data-ttu-id="45200-113">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="45200-113">_varies by context_</span></span> |
| <span data-ttu-id="45200-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="45200-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="45200-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45200-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="45200-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45200-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45200-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45200-117">Not supported.</span></span>|
|<span data-ttu-id="45200-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45200-118">Application</span></span>|<span data-ttu-id="45200-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45200-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45200-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45200-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="45200-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45200-121">Request headers</span></span>
|<span data-ttu-id="45200-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45200-122">Header</span></span>|<span data-ttu-id="45200-123">Значение</span><span class="sxs-lookup"><span data-stu-id="45200-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45200-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="45200-124">Authorization</span></span>|<span data-ttu-id="45200-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45200-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45200-126">Accept</span><span class="sxs-lookup"><span data-stu-id="45200-126">Accept</span></span>|<span data-ttu-id="45200-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45200-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45200-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45200-128">Request body</span></span>
<span data-ttu-id="45200-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45200-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45200-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="45200-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45200-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="45200-131">Property</span></span>|<span data-ttu-id="45200-132">Тип</span><span class="sxs-lookup"><span data-stu-id="45200-132">Type</span></span>|<span data-ttu-id="45200-133">Описание</span><span class="sxs-lookup"><span data-stu-id="45200-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45200-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="45200-134">deviceTag</span></span>|<span data-ttu-id="45200-135">String</span><span class="sxs-lookup"><span data-stu-id="45200-135">String</span></span>|<span data-ttu-id="45200-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="45200-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="45200-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="45200-137">Response</span></span>
<span data-ttu-id="45200-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45200-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45200-139">Пример</span><span class="sxs-lookup"><span data-stu-id="45200-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="45200-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="45200-140">Request</span></span>
<span data-ttu-id="45200-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45200-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="45200-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="45200-142">Response</span></span>
<span data-ttu-id="45200-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45200-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









