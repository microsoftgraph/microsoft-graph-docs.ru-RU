---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba6c192b69975eef2f60b09f5bb2fc43e43d51b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885192"
---
# <a name="update-reportroot"></a><span data-ttu-id="52e1c-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="52e1c-103">Update reportRoot</span></span>

> <span data-ttu-id="52e1c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52e1c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52e1c-105">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="52e1c-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52e1c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52e1c-106">Prerequisites</span></span>
<span data-ttu-id="52e1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e1c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52e1c-109">Permission type</span></span>|<span data-ttu-id="52e1c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52e1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e1c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52e1c-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="52e1c-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="52e1c-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="52e1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="52e1c-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="52e1c-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="52e1c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e1c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52e1c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52e1c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52e1c-117">Not supported.</span></span>|
|<span data-ttu-id="52e1c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52e1c-118">Application</span></span>|<span data-ttu-id="52e1c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52e1c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e1c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52e1c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="52e1c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52e1c-121">Request headers</span></span>
|<span data-ttu-id="52e1c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52e1c-122">Header</span></span>|<span data-ttu-id="52e1c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="52e1c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e1c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e1c-124">Authorization</span></span>|<span data-ttu-id="52e1c-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="52e1c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e1c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="52e1c-126">Accept</span></span>|<span data-ttu-id="52e1c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="52e1c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e1c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52e1c-128">Request body</span></span>
<span data-ttu-id="52e1c-129">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52e1c-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="52e1c-130">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="52e1c-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="52e1c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="52e1c-131">Property</span></span>|<span data-ttu-id="52e1c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="52e1c-132">Type</span></span>|<span data-ttu-id="52e1c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="52e1c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e1c-134">id</span><span class="sxs-lookup"><span data-stu-id="52e1c-134">id</span></span>|<span data-ttu-id="52e1c-135">String</span><span class="sxs-lookup"><span data-stu-id="52e1c-135">String</span></span>|<span data-ttu-id="52e1c-136">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="52e1c-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="52e1c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="52e1c-137">Response</span></span>
<span data-ttu-id="52e1c-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52e1c-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e1c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="52e1c-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="52e1c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="52e1c-140">Request</span></span>
<span data-ttu-id="52e1c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52e1c-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="52e1c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="52e1c-142">Response</span></span>
<span data-ttu-id="52e1c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="52e1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








