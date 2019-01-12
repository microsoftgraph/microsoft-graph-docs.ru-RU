---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe2d928f784eaa370c964761e54c9ea4e2c4d006
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942964"
---
# <a name="create-devicecategory"></a><span data-ttu-id="8a5a0-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8a5a0-103">Create deviceCategory</span></span>

> <span data-ttu-id="8a5a0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a5a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a5a0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a5a0-107">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8a5a0-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a5a0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8a5a0-108">Prerequisites</span></span>

<span data-ttu-id="8a5a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a5a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a5a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a5a0-111">Permission type</span></span>|<span data-ttu-id="8a5a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a5a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a5a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a5a0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8a5a0-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="8a5a0-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8a5a0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5a0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a5a0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a5a0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a5a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-117">Not supported.</span></span>|
|<span data-ttu-id="8a5a0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a5a0-118">Application</span></span>|<span data-ttu-id="8a5a0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a5a0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a5a0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="8a5a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a5a0-121">Request headers</span></span>

|<span data-ttu-id="8a5a0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a5a0-122">Header</span></span>|<span data-ttu-id="8a5a0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8a5a0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a5a0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a5a0-124">Authorization</span></span>|<span data-ttu-id="8a5a0-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8a5a0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a5a0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8a5a0-126">Accept</span></span>|<span data-ttu-id="8a5a0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8a5a0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a5a0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a5a0-128">Request body</span></span>

<span data-ttu-id="8a5a0-129">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="8a5a0-130">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="8a5a0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a5a0-131">Property</span></span>|<span data-ttu-id="8a5a0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8a5a0-132">Type</span></span>|<span data-ttu-id="8a5a0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8a5a0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a5a0-134">id</span><span class="sxs-lookup"><span data-stu-id="8a5a0-134">id</span></span>|<span data-ttu-id="8a5a0-135">String</span><span class="sxs-lookup"><span data-stu-id="8a5a0-135">String</span></span>|<span data-ttu-id="8a5a0-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-136">Unique identifier for the device category.</span></span> <span data-ttu-id="8a5a0-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-137">Read-only.</span></span>|
|<span data-ttu-id="8a5a0-138">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="8a5a0-138">**Obboarding**</span></span>|
|<span data-ttu-id="8a5a0-139">описание</span><span class="sxs-lookup"><span data-stu-id="8a5a0-139">description</span></span>|<span data-ttu-id="8a5a0-140">String</span><span class="sxs-lookup"><span data-stu-id="8a5a0-140">String</span></span>|<span data-ttu-id="8a5a0-141">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="8a5a0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8a5a0-142">displayName</span></span>|<span data-ttu-id="8a5a0-143">String</span><span class="sxs-lookup"><span data-stu-id="8a5a0-143">String</span></span>|<span data-ttu-id="8a5a0-144">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="8a5a0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a5a0-145">Response</span></span>

<span data-ttu-id="8a5a0-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a5a0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8a5a0-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a5a0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a5a0-148">Request</span></span>

<span data-ttu-id="8a5a0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-149">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="8a5a0-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a5a0-150">Response</span></span>

<span data-ttu-id="8a5a0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8a5a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



