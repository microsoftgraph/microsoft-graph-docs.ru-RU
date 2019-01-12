---
title: Обновление sideLoadingKey
description: Обновление свойства объекта sideLoadingKey.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 116034afff02ac41647d781bbd85ec6f8dcaeec4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969935"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="74bcf-103">Обновление sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="74bcf-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="74bcf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74bcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74bcf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74bcf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74bcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74bcf-107">Обновление свойства объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="74bcf-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74bcf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="74bcf-108">Prerequisites</span></span>
<span data-ttu-id="74bcf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74bcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74bcf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74bcf-111">Permission type</span></span>|<span data-ttu-id="74bcf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74bcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74bcf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74bcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74bcf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74bcf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74bcf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74bcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74bcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bcf-116">Not supported.</span></span>|
|<span data-ttu-id="74bcf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74bcf-117">Application</span></span>|<span data-ttu-id="74bcf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74bcf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74bcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="74bcf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74bcf-120">Request headers</span></span>
|<span data-ttu-id="74bcf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74bcf-121">Header</span></span>|<span data-ttu-id="74bcf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74bcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74bcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74bcf-123">Authorization</span></span>|<span data-ttu-id="74bcf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74bcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74bcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74bcf-125">Accept</span></span>|<span data-ttu-id="74bcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74bcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74bcf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74bcf-127">Request body</span></span>
<span data-ttu-id="74bcf-128">В тексте запроса укажите представление JSON для объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="74bcf-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="74bcf-129">В следующей таблице показаны свойства, которые необходимы для создания [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="74bcf-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="74bcf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74bcf-130">Property</span></span>|<span data-ttu-id="74bcf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74bcf-131">Type</span></span>|<span data-ttu-id="74bcf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74bcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74bcf-133">id</span><span class="sxs-lookup"><span data-stu-id="74bcf-133">id</span></span>|<span data-ttu-id="74bcf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="74bcf-134">String</span></span>|<span data-ttu-id="74bcf-135">Со стороны загрузка уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="74bcf-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="74bcf-136">value</span><span class="sxs-lookup"><span data-stu-id="74bcf-136">value</span></span>|<span data-ttu-id="74bcf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="74bcf-137">String</span></span>|<span data-ttu-id="74bcf-138">Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.</span><span class="sxs-lookup"><span data-stu-id="74bcf-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="74bcf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="74bcf-139">displayName</span></span>|<span data-ttu-id="74bcf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="74bcf-140">String</span></span>|<span data-ttu-id="74bcf-141">Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="74bcf-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="74bcf-142">описание</span><span class="sxs-lookup"><span data-stu-id="74bcf-142">description</span></span>|<span data-ttu-id="74bcf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="74bcf-143">String</span></span>|<span data-ttu-id="74bcf-144">Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="74bcf-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="74bcf-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="74bcf-145">totalActivation</span></span>|<span data-ttu-id="74bcf-146">Int32</span><span class="sxs-lookup"><span data-stu-id="74bcf-146">Int32</span></span>|<span data-ttu-id="74bcf-147">Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="74bcf-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="74bcf-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="74bcf-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="74bcf-149">Строка</span><span class="sxs-lookup"><span data-stu-id="74bcf-149">String</span></span>|<span data-ttu-id="74bcf-150">Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="74bcf-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="74bcf-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="74bcf-151">Response</span></span>
<span data-ttu-id="74bcf-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74bcf-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74bcf-153">Пример</span><span class="sxs-lookup"><span data-stu-id="74bcf-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="74bcf-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="74bcf-154">Request</span></span>
<span data-ttu-id="74bcf-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74bcf-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 193

{
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="74bcf-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="74bcf-156">Response</span></span>
<span data-ttu-id="74bcf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74bcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





