---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a902d341761cf56ced39a8309479ca27611ec5ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934557"
---
# <a name="update-reportroot"></a><span data-ttu-id="b794b-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="b794b-103">Update reportRoot</span></span>

> <span data-ttu-id="b794b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b794b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b794b-105">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b794b-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b794b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b794b-106">Prerequisites</span></span>
<span data-ttu-id="b794b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b794b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b794b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b794b-109">Permission type</span></span>|<span data-ttu-id="b794b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b794b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b794b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b794b-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b794b-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="b794b-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="b794b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b794b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b794b-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b794b-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b794b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b794b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b794b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b794b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b794b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b794b-117">Not supported.</span></span>|
|<span data-ttu-id="b794b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b794b-118">Application</span></span>|<span data-ttu-id="b794b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b794b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b794b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b794b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="b794b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b794b-121">Request headers</span></span>
|<span data-ttu-id="b794b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b794b-122">Header</span></span>|<span data-ttu-id="b794b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b794b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b794b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b794b-124">Authorization</span></span>|<span data-ttu-id="b794b-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b794b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b794b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b794b-126">Accept</span></span>|<span data-ttu-id="b794b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b794b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b794b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b794b-128">Request body</span></span>
<span data-ttu-id="b794b-129">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b794b-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="b794b-130">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b794b-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="b794b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b794b-131">Property</span></span>|<span data-ttu-id="b794b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b794b-132">Type</span></span>|<span data-ttu-id="b794b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b794b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b794b-134">id</span><span class="sxs-lookup"><span data-stu-id="b794b-134">id</span></span>|<span data-ttu-id="b794b-135">String</span><span class="sxs-lookup"><span data-stu-id="b794b-135">String</span></span>|<span data-ttu-id="b794b-136">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="b794b-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b794b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b794b-137">Response</span></span>
<span data-ttu-id="b794b-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b794b-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b794b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b794b-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b794b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b794b-140">Request</span></span>
<span data-ttu-id="b794b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b794b-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b794b-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="b794b-142">Response</span></span>
<span data-ttu-id="b794b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b794b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








