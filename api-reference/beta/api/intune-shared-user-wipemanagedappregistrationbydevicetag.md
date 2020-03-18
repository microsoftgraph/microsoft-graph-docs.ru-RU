---
title: Действие wipeManagedAppRegistrationByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 053d1b290111216653c0cd3e4d71fa5d01fcf8ca
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800517"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="53cdb-103">Действие wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="53cdb-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="53cdb-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53cdb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53cdb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53cdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53cdb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53cdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53cdb-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="53cdb-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53cdb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53cdb-108">Prerequisites</span></span>

<span data-ttu-id="53cdb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53cdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53cdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53cdb-111">Permission type</span></span>|<span data-ttu-id="53cdb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53cdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53cdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53cdb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="53cdb-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="53cdb-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="53cdb-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53cdb-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53cdb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53cdb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53cdb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53cdb-117">Not supported.</span></span>|
|<span data-ttu-id="53cdb-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="53cdb-118">Application</span></span>||
| <span data-ttu-id="53cdb-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="53cdb-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="53cdb-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53cdb-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53cdb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53cdb-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="53cdb-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53cdb-122">Request headers</span></span>

|<span data-ttu-id="53cdb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53cdb-123">Header</span></span>|<span data-ttu-id="53cdb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="53cdb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53cdb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53cdb-125">Authorization</span></span>|<span data-ttu-id="53cdb-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53cdb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53cdb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="53cdb-127">Accept</span></span>|<span data-ttu-id="53cdb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="53cdb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53cdb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53cdb-129">Request body</span></span>

<span data-ttu-id="53cdb-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53cdb-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="53cdb-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="53cdb-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="53cdb-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="53cdb-132">Property</span></span>|<span data-ttu-id="53cdb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="53cdb-133">Type</span></span>|<span data-ttu-id="53cdb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="53cdb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53cdb-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="53cdb-135">deviceTag</span></span>|<span data-ttu-id="53cdb-136">String</span><span class="sxs-lookup"><span data-stu-id="53cdb-136">String</span></span>|<span data-ttu-id="53cdb-137">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="53cdb-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="53cdb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="53cdb-138">Response</span></span>

<span data-ttu-id="53cdb-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="53cdb-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="53cdb-140">Пример</span><span class="sxs-lookup"><span data-stu-id="53cdb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="53cdb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="53cdb-141">Request</span></span>

<span data-ttu-id="53cdb-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53cdb-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="53cdb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="53cdb-143">Response</span></span>

<span data-ttu-id="53cdb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53cdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```













