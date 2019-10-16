---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 930300d1d657ccb795597193ab414e4248500641
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537918"
---
# <a name="update-reportroot"></a><span data-ttu-id="3559b-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="3559b-103">Update reportRoot</span></span>

> <span data-ttu-id="3559b-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3559b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3559b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3559b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3559b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3559b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3559b-107">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="3559b-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3559b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3559b-108">Prerequisites</span></span>
<span data-ttu-id="3559b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3559b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3559b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3559b-111">Permission type</span></span>|<span data-ttu-id="3559b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3559b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3559b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3559b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3559b-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="3559b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3559b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3559b-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="3559b-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="3559b-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3559b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3559b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3559b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3559b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3559b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3559b-119">Not supported.</span></span>|
|<span data-ttu-id="3559b-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="3559b-120">Application</span></span>||
| <span data-ttu-id="3559b-121">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="3559b-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3559b-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3559b-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="3559b-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="3559b-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3559b-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3559b-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3559b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3559b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="3559b-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3559b-126">Request headers</span></span>
|<span data-ttu-id="3559b-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3559b-127">Header</span></span>|<span data-ttu-id="3559b-128">Значение</span><span class="sxs-lookup"><span data-stu-id="3559b-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3559b-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3559b-129">Authorization</span></span>|<span data-ttu-id="3559b-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3559b-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3559b-131">Accept</span><span class="sxs-lookup"><span data-stu-id="3559b-131">Accept</span></span>|<span data-ttu-id="3559b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="3559b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3559b-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3559b-133">Request body</span></span>
<span data-ttu-id="3559b-134">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3559b-134">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="3559b-135">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="3559b-135">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="3559b-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="3559b-136">Property</span></span>|<span data-ttu-id="3559b-137">Тип</span><span class="sxs-lookup"><span data-stu-id="3559b-137">Type</span></span>|<span data-ttu-id="3559b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3559b-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3559b-139">id</span><span class="sxs-lookup"><span data-stu-id="3559b-139">id</span></span>|<span data-ttu-id="3559b-140">String</span><span class="sxs-lookup"><span data-stu-id="3559b-140">String</span></span>|<span data-ttu-id="3559b-141">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="3559b-141">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3559b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3559b-142">Response</span></span>
<span data-ttu-id="3559b-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3559b-143">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3559b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3559b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="3559b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3559b-145">Request</span></span>
<span data-ttu-id="3559b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3559b-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3559b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3559b-147">Response</span></span>
<span data-ttu-id="3559b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3559b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```









