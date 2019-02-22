---
title: Действие wipeManagedAppRegistrationByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef01d77a36224a9cf4d680c5cc1abfda4af5a9b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157059"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="471f1-103">Действие wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="471f1-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="471f1-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="471f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="471f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="471f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="471f1-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="471f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="471f1-107">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="471f1-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="471f1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="471f1-108">Prerequisites</span></span>

<span data-ttu-id="471f1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="471f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="471f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="471f1-111">Permission type</span></span>|<span data-ttu-id="471f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="471f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="471f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="471f1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="471f1-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="471f1-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="471f1-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="471f1-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="471f1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="471f1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="471f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="471f1-117">Not supported.</span></span>|
|<span data-ttu-id="471f1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="471f1-118">Application</span></span>|<span data-ttu-id="471f1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="471f1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="471f1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="471f1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="471f1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="471f1-121">Request headers</span></span>

|<span data-ttu-id="471f1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="471f1-122">Header</span></span>|<span data-ttu-id="471f1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="471f1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="471f1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="471f1-124">Authorization</span></span>|<span data-ttu-id="471f1-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="471f1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="471f1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="471f1-126">Accept</span></span>|<span data-ttu-id="471f1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="471f1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="471f1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="471f1-128">Request body</span></span>

<span data-ttu-id="471f1-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="471f1-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="471f1-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="471f1-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="471f1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="471f1-131">Property</span></span>|<span data-ttu-id="471f1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="471f1-132">Type</span></span>|<span data-ttu-id="471f1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="471f1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="471f1-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="471f1-134">deviceTag</span></span>|<span data-ttu-id="471f1-135">String</span><span class="sxs-lookup"><span data-stu-id="471f1-135">String</span></span>|<span data-ttu-id="471f1-136">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="471f1-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="471f1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="471f1-137">Response</span></span>

<span data-ttu-id="471f1-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="471f1-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="471f1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="471f1-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="471f1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="471f1-140">Request</span></span>

<span data-ttu-id="471f1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="471f1-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="471f1-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="471f1-142">Response</span></span>

<span data-ttu-id="471f1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="471f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






