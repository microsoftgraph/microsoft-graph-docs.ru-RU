---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08002aefd92bda80c8c5a47e261201434777cea4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962129"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="04b38-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="04b38-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="04b38-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04b38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04b38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b38-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04b38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b38-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="04b38-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b38-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04b38-108">Prerequisites</span></span>

<span data-ttu-id="04b38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b38-111">Permission type</span></span>|<span data-ttu-id="04b38-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b38-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04b38-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="04b38-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="04b38-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b38-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04b38-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b38-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b38-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b38-117">Not supported.</span></span>|
|<span data-ttu-id="04b38-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b38-118">Application</span></span>|<span data-ttu-id="04b38-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b38-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b38-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b38-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="04b38-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b38-121">Request headers</span></span>

|<span data-ttu-id="04b38-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04b38-122">Header</span></span>|<span data-ttu-id="04b38-123">Значение</span><span class="sxs-lookup"><span data-stu-id="04b38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b38-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b38-124">Authorization</span></span>|<span data-ttu-id="04b38-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b38-126">Accept</span><span class="sxs-lookup"><span data-stu-id="04b38-126">Accept</span></span>|<span data-ttu-id="04b38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="04b38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b38-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b38-128">Request body</span></span>

<span data-ttu-id="04b38-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04b38-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04b38-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="04b38-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04b38-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="04b38-131">Property</span></span>|<span data-ttu-id="04b38-132">Тип</span><span class="sxs-lookup"><span data-stu-id="04b38-132">Type</span></span>|<span data-ttu-id="04b38-133">Описание</span><span class="sxs-lookup"><span data-stu-id="04b38-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b38-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="04b38-134">deviceTag</span></span>|<span data-ttu-id="04b38-135">String</span><span class="sxs-lookup"><span data-stu-id="04b38-135">String</span></span>|<span data-ttu-id="04b38-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="04b38-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="04b38-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b38-137">Response</span></span>

<span data-ttu-id="04b38-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04b38-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04b38-139">Пример</span><span class="sxs-lookup"><span data-stu-id="04b38-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b38-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b38-140">Request</span></span>

<span data-ttu-id="04b38-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b38-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="04b38-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b38-142">Response</span></span>

<span data-ttu-id="04b38-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04b38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






