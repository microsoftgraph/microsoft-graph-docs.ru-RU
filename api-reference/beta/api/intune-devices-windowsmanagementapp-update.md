---
title: Обновление windowsManagementApp
description: Обновление свойства объекта windowsManagementApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe6412c08ba05bb26985cc5fd6a8ab0b58bc8e59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980246"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="8a24c-103">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="8a24c-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="8a24c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a24c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a24c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a24c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a24c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8a24c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a24c-107">Обновление свойства объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8a24c-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a24c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a24c-108">Prerequisites</span></span>
<span data-ttu-id="8a24c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a24c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a24c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a24c-111">Permission type</span></span>|<span data-ttu-id="8a24c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a24c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a24c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a24c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a24c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a24c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a24c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a24c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a24c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a24c-116">Not supported.</span></span>|
|<span data-ttu-id="8a24c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a24c-117">Application</span></span>|<span data-ttu-id="8a24c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a24c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a24c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a24c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="8a24c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a24c-120">Request headers</span></span>
|<span data-ttu-id="8a24c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a24c-121">Header</span></span>|<span data-ttu-id="8a24c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a24c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a24c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a24c-123">Authorization</span></span>|<span data-ttu-id="8a24c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8a24c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a24c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a24c-125">Accept</span></span>|<span data-ttu-id="8a24c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a24c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a24c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a24c-127">Request body</span></span>
<span data-ttu-id="8a24c-128">В тексте запроса укажите представление JSON для объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8a24c-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="8a24c-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a24c-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="8a24c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a24c-130">Property</span></span>|<span data-ttu-id="8a24c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a24c-131">Type</span></span>|<span data-ttu-id="8a24c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a24c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a24c-133">id</span><span class="sxs-lookup"><span data-stu-id="8a24c-133">id</span></span>|<span data-ttu-id="8a24c-134">String</span><span class="sxs-lookup"><span data-stu-id="8a24c-134">String</span></span>|<span data-ttu-id="8a24c-135">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="8a24c-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="8a24c-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="8a24c-136">availableVersion</span></span>|<span data-ttu-id="8a24c-137">String</span><span class="sxs-lookup"><span data-stu-id="8a24c-137">String</span></span>|<span data-ttu-id="8a24c-138">Управление приложения доступные версии Windows.</span><span class="sxs-lookup"><span data-stu-id="8a24c-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="8a24c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a24c-139">Response</span></span>
<span data-ttu-id="8a24c-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8a24c-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a24c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8a24c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a24c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a24c-142">Request</span></span>
<span data-ttu-id="8a24c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a24c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 53

{
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="8a24c-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a24c-144">Response</span></span>
<span data-ttu-id="8a24c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8a24c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```





